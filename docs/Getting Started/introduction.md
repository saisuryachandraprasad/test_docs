---
title: Introduction
deprecated: false
hidden: false
metadata:
  robots: index
---
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
        <th
          rowSpan="2"
          style={{
            backgroundColor: "#f3f4f6",
            fontWeight: "600",
            padding: "12px",
            textAlign: "center",
            borderRight: "1px solid #e5e7eb"
          }}
        >
          Level
        </th>

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
