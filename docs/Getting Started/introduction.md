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
      minWidth: "700px",
      tableLayout: "fixed",
      borderCollapse: "separate",
      borderSpacing: 0,
      fontSize: "14px",
      fontFamily: "Segoe UI, Arial, sans-serif",
      border: "1px solid #e5e7eb",
      borderRadius: "10px",
      overflow: "hidden"
    }}
  >
    <thead>
      <tr>
        <th
          rowSpan="2"
          style={{
            backgroundColor: "#f54562",
            color: "#ffffff",
            fontWeight: "600",
            padding: "12px",
            textAlign: "center"
          }}
        >
          Aggregation Level
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
          Aggregation Paths (Independent Sequences)
        </th>
      </tr>

      <tr>
        {["Path 1", "Path 2", "Path 3", "Path 4"].map((item) => (
                  <th
                    key={item}
                    style={{
                      backgroundColor: "#f9fafb",
                      color: "#374151",
                      fontWeight: "600",
                      padding: "10px",
                      borderBottom: "1px solid #e5e7eb"
                    }}
                  >
                    {item}
                  </th>
                ))}
      </tr>
    </thead>

    <tbody>
      <tr>
        <td style={{ padding: "10px", fontWeight: "500" }}>Level 1</td>
        <td>A</td>
        <td>E</td>
        <td>I</td>
        <td>M</td>
      </tr>

      <tr style={{ backgroundColor: "#fafafa" }}>
        <td style={{ padding: "10px", fontWeight: "500" }}>Level 2</td>
        <td>AB</td>
        <td>EF</td>
        <td>IJ</td>
        <td>MN</td>
      </tr>

      <tr>
        <td style={{ padding: "10px", fontWeight: "500" }}>Level 3</td>
        <td>ABC</td>
        <td>EFG</td>
        <td>IJK</td>
        <td>MNO</td>
      </tr>

      <tr style={{ backgroundColor: "#fafafa" }}>
        <td style={{ padding: "10px", fontWeight: "500" }}>Level 4</td>
        <td>ABCD</td>
        <td>EFGH</td>
        <td>IJKL</td>
        <td>MNOP</td>
      </tr>
    </tbody>
  </table>
</div>
