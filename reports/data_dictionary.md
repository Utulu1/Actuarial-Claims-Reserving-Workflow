| Variable           | Data Type | Business Meaning           | Used in Analysis | Comments                  |
| ------------------ | --------- | -------------------------- | ---------------- | ------------------------- |
| GRCODE             | Integer   | Insurance group identifier | Yes              | Used to filter insurers   |
| GRNAME             | Text      | Insurance group name       | Yes              | Client selection          |
| AccidentYear       | Integer   | Year claims occurred       | Yes              | Triangle rows             |
| DevelopmentYear    | Integer   | Calendar valuation year    | Yes              | Development tracking      |
| DevelopmentLag     | Integer   | Years since accident       | Yes              | Triangle columns          |
| IncurredLosses     | Integer   | Cumulative incurred losses | Yes              | Reserve estimation        |
| CumPaidLoss        | Integer   | Cumulative paid losses     | Yes              | Chain Ladder input        |
| BulkLoss           | Integer   | Bulk reserve               | Optional         | Sensitivity analysis      |
| EarnedPremNet      | Integer   | Net earned premium         | Later            | Premium adequacy analysis |
| PostedReserves2007 | Float     | Posted reserve             | Yes              | Validation benchmark      |

