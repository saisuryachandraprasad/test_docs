---
title: Test-2
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

import React from "react";

export default function ApiHomePage() {
  return (
    <div style={{ maxWidth: "1000px" }}>

      {/* HERO */}
      <div style={{ marginBottom: "50px" }}>
        <h1 style={{ fontSize: "40px", marginBottom: "8px" }}>
          Lightcast APIs
        </h1>

        <p style={{ fontSize: "18px", color: "#555", maxWidth: "720px" }}>
          Build with the world’s most trusted labor market data.
          Access structured skills, occupations, job postings, and workforce intelligence through scalable APIs.
        </p>

        <div style={{
          display: "flex",
          gap: "12px",
          flexWrap: "wrap",
          marginTop: "20px"
        }}>
          <a
            href="/docs"
            style={{
              background: "#FF5A1F",
              color: "#fff",
              padding: "12px 20px",
              borderRadius: "8px",
              fontWeight: 600,
              textDecoration: "none"
            }}
          >
            Explore Documentation
          </a>

          <a
            href="https://lightcast.io/open-skills/access"
            target="_blank"
            style={{
              border: "1px solid #FF5A1F",
              color: "#FF5A1F",
              padding: "12px 20px",
              borderRadius: "8px",
              fontWeight: 600,
              textDecoration: "none"
            }}
          >
            Get API Credentials
          </a>

          <a
            href="/reference"
            style={{
              border: "1px solid #ddd",
              padding: "12px 20px",
              borderRadius: "8px",
              fontWeight: 600,
              textDecoration: "none"
            }}
          >
            View Endpoints
          </a>
        </div>

        <div
          style={{
            height: "4px",
            width: "80px",
            background: "#FF5A1F",
            borderRadius: "4px",
            marginTop: "20px"
          }}
        />
      </div>



      {/* QUICK START */}
      <div style={{ marginBottom: "60px" }}>
        <h2>:rocket: Quick Start</h2>

        <div
          style={{
            display: "grid",
            gridTemplateColumns: "repeat(auto-fit, minmax(240px, 1fr))",
            gap: "20px",
            marginTop: "20px"
          }}
        >
          {[
            {
              title: ":blue_book: Documentation",
              text: "Explore guides, concepts, and implementation details."
            },
            {
              title: ":key: API Credentials",
              text: "Generate and manage your API keys securely."
            },
            {
              title: ":package: Postman Collection",
              text: "Test endpoints instantly with our pre-configured collection."
            },
            {
              title: ":closed_lock_with_key: Authentication Guide",
              text: "Learn how to authorize requests across APIs."
            }
          ].map((card, i) => (
            <div
              key={i}
              style={{
                border: "1px solid #eee",
                padding: "20px",
                borderRadius: "12px",
                background: "#fff",
                transition: "0.2s ease"
              }}
            >
              <h4 style={{ marginBottom: "8px" }}>{card.title}</h4>
              <p style={{ fontSize: "14px", color: "#555" }}>
                {card.text}
              </p>
            </div>
          ))}
        </div>
      </div>



      {/* WHAT YOU CAN BUILD */}
      <div style={{ marginBottom: "60px" }}>
        <h2>:bar_chart: What You Can Build</h2>

        <ul style={{ marginTop: "16px", lineHeight: "1.8" }}>
          <li>Workforce analytics dashboards</li>
          <li>Skill intelligence platforms</li>
          <li>Job-to-skill mapping tools</li>
          <li>Education alignment systems</li>
          <li>Regional labor market reporting</li>
          <li>Talent supply & demand monitoring</li>
        </ul>
      </div>



      {/* TESTIMONIAL */}
      <div style={{ marginBottom: "60px" }}>
        <h2>Trusted by Industry Leaders</h2>

        <div
          style={{
            borderLeft: "4px solid #FF5A1F",
            paddingLeft: "18px",
            fontStyle: "italic",
            color: "#555",
            marginTop: "20px"
          }}
        >
          “Lightcast has the world’s best labour market data, and along with the excellent customer service we get, this means we are able to develop software solutions that bring genuinely useful skills and talent insights to our customers.”
          <br /><br />
          — John Guy, Co-Founder @ Simply
        </div>
      </div>



      {/* LEGACY LINK */}
      <div style={{ marginBottom: "40px" }}>
        <h2>Legacy Documentation</h2>
        <p>
          We are actively migrating content to this new portal.
          For APIs not yet available here, visit:
        </p>
        <a
          href="https://docs.lightcast.dev"
          target="_blank"
          style={{ color: "#FF5A1F", fontWeight: 600 }}
        >
          https://docs.lightcast.dev
        </a>
      </div>

    </div>
  );
}
