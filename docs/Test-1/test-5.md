---
title: Test
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

import React, { useState } from "react";

export default function FAQAccordion() {
  const [activeIndex, setActiveIndex] = useState(null);

  const faqData = [
    {
      number: "01/",
      question: "How long can I use this plan?",
      answer:
        "You can use this plan as long as your eligibility remains valid."
    },
    {
      number: "02/",
      question:
        "How long does it take to be approved as a qualified academic institution?",
      answer:
        "Approval timelines vary depending on verification requirements."
    },
    {
      number: "03/",
      question: "What can I do if I'm not eligible?",
      answer:
        "You may explore alternative subscription plans available for individuals or businesses."
    },
    {
      number: "04/",
      question:
        "What is the difference between Office 365 and Microsoft 365 Education?",
      answer:
        "Microsoft 365 Education includes additional security and collaboration features tailored for academic institutions."
    }
  ];

  const toggleItem = (index) => {
    setActiveIndex(activeIndex === index ? null : index);
  };

  return (
    <div style={{ maxWidth: "900px" }}>
      {faqData.map((item, index) => {
        const isOpen = activeIndex === index;

        return (
          <div key={index} style={{ borderBottom: "1px solid #e1e1e1" }}>
            <button
              onClick={() => toggleItem(index)}
              aria-expanded={isOpen}
              style={{
                width: "100%",
                background: "none",
                border: "none",
                padding: "20px 0",
                display: "flex",
                alignItems: "center",
                textAlign: "left",
                cursor: "pointer",
                fontSize: "16px",
                fontWeight: 600
              }}
            >
              <span style={{ marginRight: "12px", color: "#f54562", minWidth: "40px" }}>
                {item.number}
              </span>

              <span style={{ flex: 1 }}>
                {item.question}
              </span>

              <span
                style={{
                  width: "36px",
                  height: "36px",
                  background: "#f54562",
                  color: "#fff",
                  borderRadius: "8px",
                  display: "flex",
                  alignItems: "center",
                  justifyContent: "center",
                  fontSize: "18px"
                }}
              >
                {isOpen ? "–" : "+"}
              </span>
            </button>

            <div
              style={{
                maxHeight: isOpen ? "500px" : "0px",
                overflow: "hidden",
                transition: "max-height 0.3s ease"
              }}
            >
              <p style={{ margin: "0 0 20px 0", fontSize: "14px" }}>
                {item.answer}
              </p>
            </div>
          </div>
        );
      })}
    </div>
  );
}
