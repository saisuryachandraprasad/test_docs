---
title: Introduction
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

<table style={{ borderCollapse: "collapse", textAlign: "center", width: "100%" }}>
  <thead>
    <tr>
      <th style={{ border: "1px solid #ccc" }} />

      <th style={{ border: "1px solid #ccc" }} />

      <th colSpan="4" style={{ border: "1px solid #ccc", backgroundColor: "#93c47d" }}>
        Aggregation Path
      </th>
    </tr>

    <tr>
      <th style={{ border: "1px solid #ccc" }} />

      <th style={{ border: "1px solid #ccc" }} />

      <th style={{ border: "1px solid #ccc" }}>1</th>
      <th style={{ border: "1px solid #ccc" }}>2</th>
      <th style={{ border: "1px solid #ccc" }}>3</th>
      <th style={{ border: "1px solid #ccc" }}>4</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td
        rowSpan="4"
        style={{
          border: "1px solid #ccc",
          backgroundColor: "#93c47d",
          fontWeight: "bold"
        }}
      >
        Level
      </td>

      <td style={{ border: "1px solid #ccc" }}>1</td>
      <td style={{ border: "1px solid #ccc" }}>A</td>
      <td style={{ border: "1px solid #ccc" }}>E</td>
      <td style={{ border: "1px solid #ccc" }}>I</td>
      <td style={{ border: "1px solid #ccc" }}>M</td>
    </tr>

    <tr>
      <td style={{ border: "1px solid #ccc" }}>2</td>
      <td>AB</td>
      <td>EF</td>
      <td>IJ</td>
      <td>MN</td>
    </tr>

    <tr>
      <td style={{ border: "1px solid #ccc" }}>3</td>
      <td>ABC</td>
      <td>EFG</td>
      <td>IJK</td>
      <td>MNO</td>
    </tr>

    <tr>
      <td style={{ border: "1px solid #ccc" }}>4</td>
      <td>ABCD</td>
      <td>EFGH</td>
      <td>IJKL</td>
      <td>MNOP</td>
    </tr>
  </tbody>
</table>

<br />

<br />

<br />

<div style={{ overflowX: "auto", margin: "16px 0" }}>
  <table
    style={{
      borderCollapse: "separate",
      borderSpacing: 0,
      width: "100%",
      fontSize: "14px",
      fontFamily: "Segoe UI, Arial, sans-serif",
      border: "1px solid #e5e7eb",
      borderRadius: "10px",
      overflow: "hidden",
      boxShadow: "0 2px 8px rgba(0,0,0,0.05)"
    }}
  >
    <thead>
      <tr>
        <th style={{ padding: "12px" }} />

        <th style={{ padding: "12px" }} />

        <th
          colSpan="4"
          style={{
            backgroundColor: "#4f46e5",
            color: "#ffffff",
            fontWeight: "600",
            fontSize: "15px",
            padding: "14px",
            textAlign: "center"
          }}
        >
          Aggregation Path
        </th>
      </tr>

      <tr>
        <th style={{ padding: "10px" }} />

        <th style={{ padding: "10px" }} />

        {["1", "2", "3", "4"].map((item) => (
                  <th
                    key={item}
                    style={{
                      backgroundColor: "#eef2ff",
                      color: "#3730a3",
                      fontWeight: "600",
                      padding: "10px"
                    }}
                  >
                    {item}
                  </th>
                ))}
      </tr>
    </thead>

    <tbody>
      <tr>
        <td
          rowSpan="4"
          style={{
            backgroundColor: "#f3f4f6",
            fontWeight: "600",
            textAlign: "center",
            verticalAlign: "middle",
            padding: "12px",
            borderRight: "1px solid #e5e7eb"
          }}
        >
          Level
        </td>

        <td style={{ padding: "10px", fontWeight: "500" }}>1</td>
        <td style={{ padding: "10px" }}>A</td>
        <td style={{ padding: "10px" }}>E</td>
        <td style={{ padding: "10px" }}>I</td>
        <td style={{ padding: "10px" }}>M</td>
      </tr>

      <tr style={{ backgroundColor: "#fafafa" }}>
        <td style={{ padding: "10px", fontWeight: "500" }}>2</td>
        <td>AB</td>
        <td>EF</td>
        <td>IJ</td>
        <td>MN</td>
      </tr>

      <tr>
        <td style={{ padding: "10px", fontWeight: "500" }}>3</td>
        <td>ABC</td>
        <td>EFG</td>
        <td>IJK</td>
        <td>MNO</td>
      </tr>

      <tr style={{ backgroundColor: "#fafafa" }}>
        <td style={{ padding: "10px", fontWeight: "500" }}>4</td>
        <td>ABCD</td>
        <td>EFGH</td>
        <td>IJKL</td>
        <td>MNOP</td>
      </tr>
    </tbody>
  </table>
</div>
