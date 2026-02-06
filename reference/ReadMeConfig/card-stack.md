---
title: Card Stack Custom Component
excerpt: Build an interactive stacked card layout as a ReadMe custom component.
api_config: getting-started
hidden: false
---

This custom component recreates the stacked card interaction from the provided HTML/CSS example and is ready to paste into **ReadMe > Custom Components**. It includes basic error handling to surface helpful messages when required props are missing.

## React component

```jsx
import React, { useMemo } from 'react';

export default function CardStack({ cards }) {
  const normalizedCards = useMemo(() => {
    if (!Array.isArray(cards)) {
      return { error: 'Expected the `cards` prop to be an array.' };
    }

    if (cards.length === 0) {
      return { error: 'Add at least one card title to render the stack.' };
    }

    return { data: cards };
  }, [cards]);

  if (normalizedCards.error) {
    return (
      <div style={{
        backgroundColor: '#27131a',
        border: '1px solid #7a1f3d',
        borderRadius: 8,
        color: '#f6c4d2',
        fontFamily: 'Open Sans, sans-serif',
        padding: '12px 16px',
      }}>
        <strong>CardStack error:</strong> {normalizedCards.error}
      </div>
    );
  }

  return (
    <div className="card-stack" aria-label="Stacked cards">
      {normalizedCards.data.map((title, index) => (
        <div className="card-stack__card" key={`${title}-${index}`}>
          <h3 className="card-stack__title">{title}</h3>
          <div className="card-stack__bar">
            <div className="card-stack__bar-empty" />
            <div className="card-stack__bar-filled" />
          </div>
          <div className="card-stack__circle">
            <svg version="1.1" xmlns="http://www.w3.org/2000/svg">
              <circle className="card-stack__stroke" cx="60" cy="60" r="50" />
            </svg>
          </div>
        </div>
      ))}

      <style>
        {`
          @import url('https://fonts.googleapis.com/css?family=Open+Sans:300i,400');

          .card-stack {
            position: relative;
            display: flex;
            height: 300px;
            width: 600px;
            max-width: 100%;
            margin: 60px auto 0;
            font-family: 'Open Sans', sans-serif;
          }

          .card-stack__card {
            display: flex;
            height: 280px;
            width: 200px;
            background-color: #17141d;
            border-radius: 10px;
            box-shadow: -1rem 0 3rem #000;
            transition: 0.4s ease-out;
            position: relative;
            left: 0;
          }

          .card-stack__card:not(:first-child) {
            margin-left: -50px;
          }

          .card-stack__card:hover {
            transform: translateY(-20px);
            transition: 0.4s ease-out;
          }

          .card-stack__card:hover ~ .card-stack__card {
            position: relative;
            left: 50px;
            transition: 0.4s ease-out;
          }

          .card-stack__title {
            color: white;
            font-weight: 300;
            position: absolute;
            left: 20px;
            top: 15px;
          }

          .card-stack__bar {
            position: absolute;
            top: 100px;
            left: 20px;
            height: 5px;
            width: 150px;
          }

          .card-stack__bar-empty {
            background-color: #2e3033;
            width: 100%;
            height: 100%;
          }

          .card-stack__bar-filled {
            position: absolute;
            top: 0;
            z-index: 3;
            width: 0;
            height: 100%;
            background: rgb(0,154,217);
            background: linear-gradient(90deg, rgba(0,154,217,1) 0%, rgba(217,147,0,1) 65%, rgba(255,186,0,1) 100%);
            transition: 0.6s ease-out;
          }

          .card-stack__card:hover .card-stack__bar-filled {
            width: 120px;
            transition: 0.4s ease-out;
          }

          .card-stack__circle {
            position: absolute;
            top: 150px;
            left: calc(50% - 60px);
          }

          .card-stack__stroke {
            stroke: white;
            stroke-dasharray: 360;
            stroke-dashoffset: 360;
            transition: 0.6s ease-out;
          }

          .card-stack__card:hover .card-stack__stroke {
            stroke-dashoffset: 100;
            transition: 0.6s ease-out;
          }

          .card-stack svg {
            fill: #17141d;
            stroke-width: 2px;
          }
        `}
      </style>
    </div>
  );
}
```

## Usage example

```jsx
<CardStack cards={["Card 1", "Card 2", "Card 3", "Card 4"]} />
```

## Error handling behavior

If the `cards` prop is missing, not an array, or empty, the component renders a clear error message in place of the cards. This helps authors spot configuration issues directly in the ReadMe page without crashing the rest of the content.
