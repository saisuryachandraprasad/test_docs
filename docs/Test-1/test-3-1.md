---
title: Test-3
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

import React, { useState, useEffect } from "react";

export default function ApiHomePage() {
  const brand = "#f54562";
  const [hubUrl, setHubUrl] = useState("/docs");

  useEffect(() => {
    if (typeof window !== "undefined" && window.readme?.variables?.base_url) {
      setHubUrl(window.readme.variables.base_url);
    }
  }, []);

  // Animation constants
  const transition = "all 0.3s cubic-bezier(0.4, 0, 0.2, 1)";

  return (
    <div
      style={{
        maxWidth: "1000px",
        fontFamily: "'Inter', system-ui, -apple-system, sans-serif",
        lineHeight: 1.6,
        color: "#1a1a1a",
        padding: "20px 0"
      }}
    >
      {/* HERO SECTION */}
      <div style={{ marginBottom: "60px" }}>
        <p
          style={{
            fontSize: "18px",
            color: "#4b5563",
            maxWidth: "720px",
            marginBottom: "32px",
            fontWeight: "400"
          }}
        >
          Build with the world’s most trusted labor market data.
          Access structured skills, occupations, job postings, and workforce intelligence through scalable APIs.
        </p>

        <div style={{ display: "flex", gap: "16px", flexWrap: "wrap", alignItems: "center" }}>
          
          {/* PRIMARY BUTTON */}
          <a
            href={hubUrl}
            onMouseEnter={(e) => {
              e.currentTarget.style.backgroundColor = "#d43a52";
              e.currentTarget.style.transform = "translateY(-2px)";
              e.currentTarget.style.boxShadow = "0 4px 12px rgba(245, 69, 98, 0.3)";
            }}
            onMouseLeave={(e) => {
              e.currentTarget.style.backgroundColor = brand;
              e.currentTarget.style.transform = "translateY(0)";
              e.currentTarget.style.boxShadow = "none";
            }}
            style={{
              backgroundColor: brand,
              color: "#fff",
              padding: "12px 28px",
              borderRadius: "12px",
              fontWeight: "600",
              fontSize: "14px",
              textDecoration: "none",
              display: "inline-flex",
              alignItems: "center",
              transition
            }}
          >
            Postman Collection <span style={{ marginLeft: "10px", fontSize: "18px" }}>→</span>
          </a>

          {/* SECONDARY BUTTON: Postman */}
          <a
            href="#"
            onMouseEnter={(e) => {
              e.currentTarget.style.backgroundColor = "rgba(245, 69, 98, 0.05)";
              e.currentTarget.style.borderColor = brand;
              e.currentTarget.style.transform = "translateY(-2px)";
            }}
            onMouseLeave={(e) => {
              e.currentTarget.style.backgroundColor = "transparent";
              e.currentTarget.style.borderColor = "#e5e7eb";
              e.currentTarget.style.transform = "translateY(0)";
            }}
            style={{
              border: "1px solid #e5e7eb",
              color: "#374151",
              padding: "12px 28px",
              borderRadius: "12px",
              fontWeight: "600",
              fontSize: "15px",
              textDecoration: "none",
              display: "inline-flex",
              alignItems: "center",
              transition
            }}
          >
            View Endpoints <span style={{ marginLeft: "10px", opacity: 0.5 }}>↗</span>
          </a>
        </div>
      </div>

      {/* QUICK START CARDS */}
      <div style={{ marginBottom: "60px" }}>
        <h2 style={{ fontSize: "22px", fontWeight: 700, marginBottom: "28px", letterSpacing: "-0.02em" }}>
          Quick Start
        </h2>

        <div
          style={{
            display: "grid",
            gridTemplateColumns: "repeat(auto-fit, minmax(240px, 1fr))",
            gap: "24px"
          }}
        >
          {[
            { title: "📘 Documentation", text: "Explore guides, concepts, and implementation details.", link: "/docs" },
            { title: "🔑 API Credentials", text: "Generate and manage your API keys securely.", link: "https://lightcast.io/open-skills/access" },
            { title: "📦 Postman Collection", text: "Test endpoints instantly with our pre-configured collection.", link: "#" },
            { title: "🔐 Authentication", text: "Learn how to authorize requests across APIs.", link: "/docs/authentication" }
          ].map((card, i) => (
            <a key={i} href={card.link} style={{ textDecoration: 'none', color: 'inherit' }}>
              <div
                onMouseOver={(e) => {
                  e.currentTarget.style.borderColor = brand;
                  e.currentTarget.style.boxShadow = "0 12px 24px rgba(0,0,0,0.06)";
                  e.currentTarget.style.transform = "translateY(-4px)";
                }}
                onMouseOut={(e) => {
                  e.currentTarget.style.borderColor = "#f3f4f6";
                  e.currentTarget.style.boxShadow = "none";
                  e.currentTarget.style.transform = "translateY(0)";
                }}
                style={{
                  border: "1px solid #f3f4f6",
                  padding: "28px",
                  borderRadius: "16px",
                  background: "#fff",
                  height: "100%",
                  transition,
                  cursor: "pointer"
                }}
              >
                <h4 style={{ marginBottom: "12px", fontSize: "18px", fontWeight: 700 }}>{card.title}</h4>
                <p style={{ fontSize: "16px", color: "#6b7280", lineHeight: 1.6, margin: 0 }}>{card.text}</p>
              </div>
            </a>
          ))}
        </div>
      </div>      

      {/* TESTIMONIAL SECTION */}
      <div style={{ marginBottom: "60px" }}>
        <h2 style={{ fontSize: "22px", fontWeight: 700, marginBottom: "28px", letterSpacing: "-0.02em" }}>
          Customer Success
        </h2>
        <div
          style={{
            background: "linear-gradient(145deg, #ffffff, #f9fafb)",
            padding: "32px",
            borderRadius: "20px",
            border: "1px solid #f3f4f6",
            position: "relative",
            maxWidth: "800px"
          }}
        >
          <div style={{ color: brand, fontSize: "40px", position: "absolute", top: "10px", left: "20px", opacity: 0.1, fontFamily: "serif" }}>“</div>
          <p style={{ fontStyle: "italic", color: "#4b5563", fontSize: "15px", position: "relative", zIndex: 1, margin: 0 }}>
            Lightcast has the world’s best labour market data, allowing us to develop
            solutions that bring genuinely useful insights to our customers.
          </p>
          <div style={{ marginTop: "20px", display: "flex", alignItems: "center", gap: "12px" }}>
            <div style={{ width: "32px", height: "3px", background: brand, borderRadius: "2px" }}></div>
            <span style={{ fontWeight: 700, fontSize: "12px", color: "#111827", textTransform: "uppercase", letterSpacing: "0.05em" }}>
              John Guy — Simply
            </span>
          </div>
        </div>
      </div>
    </div>
  );
}
