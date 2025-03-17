## bulldozer-price-prediction-model

## Data Dictionary

| **Variable**                 | **Description** |
|------------------------------|----------------|
| `SalesID`                    | Unique identifier of a particular sale of a machine at auction |
| `MachineID`                  | Identifier for a particular machine; machines may have multiple sales |
| `ModelID`                    | Identifier for a unique machine model (i.e. `fiModelDesc`) |
| `datasource`                 | Source of the sale record; some sources are more diligent about reporting attributes of the machine than others. A particular datasource may report on multiple `auctioneerID`s. |
| `auctioneerID`               | Identifier of a particular auctioneer, i.e., the company that sold the machine at auction. Not the same as `datasource`. |
| `YearMade`                   | Year of manufacturer of the machine |
| `MachineHoursCurrentMeter`    | Current usage of the machine in hours at the time of sale (`saledate`); null or 0 means no hours were reported for that sale |
| `UsageBand`                  | Value (`low`, `medium`, `high`) calculated by comparing this particular machine’s hours to the average usage for the `fiBaseModel`. E.g., "Low" means this machine has fewer hours relative to the model average. |
| `Saledate`                   | Time of sale |
| `Saleprice`                  | Cost of sale in USD |
| `fiModelDesc`                | Description of a unique machine model (`fiBaseModel` + `fiSecondaryDesc` + `fiModelSeries` + `fiModelDescriptor`) |
| `ProductSize`                | The size class grouping for a product group. Subsets within the product group. |
| `State`                      | US State in which the sale occurred |
| `ProductGroup`               | Identifier for top-level hierarchical grouping of `fiModelDesc` |
| `Drive_System`               | Machine configuration; typically describes whether 2 or 4-wheel drive |
| `Transmission`               | Describes type of transmission (e.g., automatic or manual) |
| `Engine_Horsepower`          | Engine horsepower rating |
| `Hydraulics`                 | Type of hydraulics system |
| `Tire_Size`                  | Size of primary tires |
| `Coupler`                    | Type of implement interface |
| `Blade_Type`                 | Describes type of blade |
| `Steering_Controls`          | Describes operator control configuration |