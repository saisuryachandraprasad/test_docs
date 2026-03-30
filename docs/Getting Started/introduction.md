---
title: Introduction
deprecated: false
hidden: false
metadata:
  robots: index
---
{(() => {
  const baseCell = {
    textAlign: "center",
    padding: "12px",
    borderRight: "1px solid #d1d5db",
    borderBottom: "1px solid #d1d5db"
  };

  const headerCell = {
    ...baseCell,
    backgroundColor: "#e5e7eb",
    color: "#6b7280",
    fontWeight: "600"
  };

  const rowHeader = {
    ...baseCell,
    backgroundColor: "#f9fafb",
    fontWeight: "600",
    padding: "10px"
  };

  return (
    <div
      style={{
        overflowX: "auto",
        borderRadius: "12px",
        overflow: "hidden",
        border: "1px solid #d1d5db"
      }}
    >
      <table
        style={{
          width: "100%",
          minWidth: "720px",
          borderCollapse: "separate",
          borderSpacing: 0,
          tableLayout: "fixed",
          fontFamily: "Segoe UI, Arial, sans-serif",
          fontSize: "14px"
        }}
      >
        <thead>
          <tr>
            <th style={{ width: "60px", backgroundColor: "#f3f4f6" }}></th>
            <th style={{ width: "60px", backgroundColor: "#f3f4f6" }}></th>

            <th
              colSpan="4"
              style={{
                backgroundColor: "#f54562",
                color: "#fff",
                fontWeight: "700",
                padding: "14px"
              }}
            >
              AGGREGATION PATH
            </th>
          </tr>

          <tr>
            <th style={{ backgroundColor: "#f3f4f6" }}></th>
            <th style={{ backgroundColor: "#f3f4f6" }}></th>

            {["1", "2", "3", "4"].map((n) => (
              <th key={n} style={headerCell}>
                {n}
              </th>
            ))}
          </tr>
        </thead>

        <tbody>
          {[
            ["1", "A", "E", "I", "M"],
            ["2", "AB", "EF", "IJ", "MN"],
            ["3", "ABC", "EFG", "IJK", "MNO"],
            ["4", "ABCD", "EFGH", "IJKL", "MNOP"]
          ].map((row, i) => (
            <tr key={i}>
              {i === 0 && (
                <td
                  rowSpan="4"
                  style={{
                    backgroundColor: "#f54562",
                    color: "#fff",
                    fontWeight: "700",
                    writingMode: "vertical-rl",
                    transform: "rotate(180deg)",
                    borderRight: "1px solid #d1d5db"
                  }}
                >
                  LEVEL
                </td>
              )}

              <td style={rowHeader}>{row[0]}</td>

              {row.slice(1).map((val, idx) => (
                <td
                  key={idx}
                  style={{
                    ...baseCell,
                    fontWeight: i === 0 ? "400" : "600",
                    borderRight: idx === 3 ? "none" : baseCell.borderRight
                  }}
                >
                  {val}
                </td>
              ))}
            </tr>
          ))}
        </tbody>
      </table>
    </div>
  );
})()}
