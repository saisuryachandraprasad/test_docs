---
title: Test-3
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

import React from "react";

export default function Hero() {
  return (
    <div
      style={{
        padding: "56px 48px",
        borderRadius: "20px",
        background: "linear-gradient(135deg, #FFF5F7 0%, #FFFFFF 100%)",
        border: "1px solid #FFE3E8",
        marginBottom: "56px",
        maxWidth: "1100px"
      }}
    >
      <h1
        style={{
          fontSize: "26px",
          marginBottom: "14px",
          fontWeight: 600,
          letterSpacing: "-0.3px",
          color: "#111"
        }}
      >
        Lightcast APIs
      </h1>

      <p
        style={{
          fontSize: "15px",
          lineHeight: 1.7,
          color: "#555",
          maxWidth: "640px",
          marginBottom: "28px"
        }}
      >
        Explore endpoints, test requests directly in the browser, and integrate
        trusted labor market data into your applications.
      </p>

      <a
        href="#authentication"
        style={{
          display: "inline-block",
          padding: "10px 20px",
          background: "#F54562",
          color: "#fff",
          borderRadius: "10px",
          textDecoration: "none",
          fontSize: "14px",
          fontWeight: 500
        }}
      >
        Get Started →
      </a>
    </div>
  );
}
