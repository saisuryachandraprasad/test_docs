---
title: Introduction
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

<div style={{ overflowX: "auto" }}>
  <table
    style={{
      width: "100%",
      minWidth: "720px",
      borderCollapse: "collapse",
      tableLayout: "fixed",
      fontFamily: "Segoe UI, Arial, sans-serif",
      fontSize: "14px"
    }}
  >
    <thead>
      <tr>
        <th style={{ width: "60px", backgroundColor: "#f3f4f6" }} />

        <th style={{ width: "60px", backgroundColor: "#f3f4f6" }} />

        <th
          colSpan="4"
          style={{
            backgroundColor: "#f54562",
            color: "#fff",
            fontWeight: "700",
            letterSpacing: "0.5px",
            padding: "14px",
            textAlign: "center"
          }}
        >
          AGGREGATION PATH
        </th>
      </tr>

      <tr>
        <th style={{ backgroundColor: "#f3f4f6" }} />

        <th style={{ backgroundColor: "#f3f4f6" }} />

        {["1", "2", "3", "4"].map((item) => (
                  <th
                    key={item}
                    style={{
                      backgroundColor: "#e5e7eb",
                      color: "#6b7280",
                      fontWeight: "600",
                      padding: "10px",
                      textAlign: "center",
                      border: "1px solid #d1d5db"
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
            backgroundColor: "#f54562",
            color: "#ffffff",
            fontWeight: "700",
            textAlign: "center",
            writingMode: "vertical-rl",
            transform: "rotate(180deg)",
            letterSpacing: "1px",
            border: "1px solid #d1d5db"
          }}
        >
          LEVEL
        </td>

        <td
          style={{
            textAlign: "center",
            fontWeight: "600",
            backgroundColor: "#f9fafb",
            border: "1px solid #d1d5db"
          }}
        >
          1
        </td>

        <td style={{ textAlign: "center", padding: "12px", border: "1px solid #d1d5db" }}>A</td>
        <td style={{ textAlign: "center", padding: "12px", border: "1px solid #d1d5db" }}>E</td>
        <td style={{ textAlign: "center", padding: "12px", border: "1px solid #d1d5db" }}>I</td>
        <td style={{ textAlign: "center", padding: "12px", border: "1px solid #d1d5db" }}>M</td>
      </tr>

      <tr>
        <td style={{ textAlign: "center", fontWeight: "600", backgroundColor: "#f9fafb", border: "1px solid #d1d5db" }}>2</td>

        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>AB</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>EF</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>IJ</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>MN</td>
      </tr>

      <tr>
        <td style={{ textAlign: "center", fontWeight: "600", backgroundColor: "#f9fafb", border: "1px solid #d1d5db" }}>3</td>

        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>ABC</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>EFG</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>IJK</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>MNO</td>
      </tr>

      <tr>
        <td style={{ textAlign: "center", fontWeight: "600", backgroundColor: "#f9fafb", border: "1px solid #d1d5db" }}>4</td>

        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>ABCD</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>EFGH</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>IJKL</td>
        <td style={{ textAlign: "center", padding: "12px", fontWeight: "600", border: "1px solid #d1d5db" }}>MNOP</td>
      </tr>
    </tbody>
  </table>
</div>
