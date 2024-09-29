<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chemical Invoices</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
        }
        table, th, td {
            border: 1px solid black;
        }
        th, td {
            padding: 10px;
            text-align: left;
        }
        th {
            cursor: pointer;
        }
    </style>
</head>
<body>

    <h1>Chemical Supplies</h1>
    <table id="chemicalTable">
        <thead>
            <tr>
                <th>ID</th>
                <th>Chemical Name</th>
                <th>Vendor</th>
                <th>Density</th>
                <th>Viscosity</th>
                <th>Packaging</th>
                <th>Pack Size</th>
                <th>Unit</th>
                <th>Quantity</th>
            </tr>
        </thead>
        <tbody id="tableBody">
            <!-- Rows will be inserted here via JavaScript -->
        </tbody>
    </table>

    <script>
        // JSON array containing 15 chemical invoice records
        const chemicalData = [
            {id: 1, chemicalName: 'Ammonium Persulfate', vendor: 'LG Chem', density: 3525.92, viscosity: 60.63, packaging: 'Bag', packSize: 100, unit: 'kg', quantity: 6495.18},
            {id: 2, chemicalName: 'Caustic Potash', vendor: 'Formosa', density: 3172.15, viscosity: 48.22, packaging: 'Bag', packSize: 100, unit: 'kg', quantity: 8751.90},
            {id: 3, chemicalName: 'Dimethylaminopropylamino', vendor: 'LG Chem', density: 8435.37, viscosity: 12.62, packaging: 'Barrel', packSize: 75, unit: 'L', quantity: 5964.61},
            {id: 4, chemicalName: 'Mono Ammonium Phosphate', vendor: 'Sinopec', density: 1597.65, viscosity: 76.51, packaging: 'Bag', packSize: 105, unit: 'kg', quantity: 8183.73},
            {id: 5, chemicalName: 'Ferric Nitrate', vendor: 'DowDuPont', density: 364.04, viscosity: 14.90, packaging: 'Bag', packSize: 105, unit: 'kg', quantity: 4154.33},
            {id: 6, chemicalName: 'n-Pentane', vendor: 'Sinopec', density: 4535.26, viscosity: 66.76, packaging: 'N/A', packSize: 'N/A', unit: 't', quantity: 6272.34},
            {id: 7, chemicalName: 'Glycol Ether PM', vendor: 'LG Chem', density: 6495.18, viscosity: 72.12, packaging: 'Bag', packSize: 250, unit: 'kg', quantity: 8749.54},
            {id: 8, chemicalName: 'Acetone', vendor: 'Formosa', density: 791.00, viscosity: 32.61, packaging: 'Drum', packSize: 200, unit: 'L', quantity: 1023.45},
            {id: 9, chemicalName: 'Ethyl Alcohol', vendor: 'DowDuPont', density: 789.00, viscosity: 34.87, packaging: 'Barrel', packSize: 150, unit: 'L', quantity: 5623.76},
            {id: 10, chemicalName: 'Sodium Hydroxide', vendor: 'Sinopec', density: 2135.45, viscosity: 40.95, packaging: 'Bag', packSize: 50, unit: 'kg', quantity: 1546.78},
            {id: 11, chemicalName: 'Benzene', vendor: 'Formosa', density: 874.12, viscosity: 35.76, packaging: 'Drum', packSize: 200, unit: 'L', quantity: 9532.21},
            {id: 12, chemicalName: 'Toluene', vendor: 'LG Chem', density: 867.10, viscosity: 24.51, packaging: 'Barrel', packSize: 100, unit: 'L', quantity: 6478.92},
            {id: 13, chemicalName: 'Sulfuric Acid', vendor: 'Sinopec', density: 1834.50, viscosity: 45.75, packaging: 'Bag', packSize: 125, unit: 'kg', quantity: 8731.24},
            {id: 14, chemicalName: 'Phosphoric Acid', vendor: 'DowDuPont', density: 1845.70, viscosity: 50.31, packaging: 'Bag', packSize: 150, unit: 'kg', quantity: 5273.14},
            {id: 15, chemicalName: 'Hydrogen Peroxide', vendor: 'Formosa', density: 1440.50, viscosity: 37.14, packaging: 'Barrel', packSize: 80, unit: 'L', quantity: 3948.65}
        ];

        // Function to populate the table
        function populateTable(data) {
            const tableBody = document.getElementById('tableBody');
            tableBody.innerHTML = ''; // Clear the table body

            data.forEach((row) => {
                const tr = document.createElement('tr');
                tr.innerHTML = `
                    <td>${row.id}</td>
                    <td>${row.chemicalName}</td>
                    <td>${row.vendor}</td>
                    <td>${row.density}</td>
                    <td>${row.viscosity}</td>
                    <td>${row.packaging}</td>
                    <td>${row.packSize}</td>
                    <td>${row.unit}</td>
                    <td>${row.quantity}</td>
                `;
                tableBody.appendChild(tr);
            });
        }

        // Populate table on page load
        document.addEventListener('DOMContentLoaded', () => {
            populateTable(chemicalData);
        });
    </script>

</body>
</html>
