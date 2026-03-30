---
title: Introduction
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

<div
  style={{
    width: "100%",
    margin: "0",
    padding: "0",
    overflowX: "auto"
  }}
>
  <table
    style={{
      width: "100%",
      minWidth: "700px",
      tableLayout: "fixed",
      borderCollapse: "separate",
      borderSpacing: 0,
      fontSize: "14px",
      fontFamily: "Segoe UI, Arial, sans-serif",
      border: "1px solid #e5e7eb",
      borderRadius: "10px",
      overflow: "hidden",
      boxShadow: "0 2px 6px rgba(0,0,0,0.04)"
    }}
  >
    <thead>
      <tr>
        <th
          rowSpan="2"
          style={{
            width: "120px",
            backgroundColor: "#f9fafb",
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
            backgroundColor: "#f54562",
            color: "#ffffff",
            fontWeight: "600",
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
                      width: "25%",
                      backgroundColor: "#ffe4e8",
                      color: "#b91c1c",
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

      <tr style={{ backgroundColor: "#fff5f6" }}>
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

      <tr style={{ backgroundColor: "#fff5f6" }}>
        <td style={{ padding: "10px", fontWeight: "500" }}>4</td>
        <td>ABCD</td>
        <td>EFGH</td>
        <td>IJKL</td>
        <td>MNOP</td>
      </tr>
    </tbody>
  </table>
</div>
