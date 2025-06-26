<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roblox Fast Flags</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #0d1117;
            color: #c9d1d9;
        }
        .container {
            max-width: 1200px;
            margin: auto;
        }
        .category {
            margin-bottom: 30px;
            background-color: #161b22;
            padding: 20px;
            border-radius: 6px;
        }
        .category h2 {
            color: #58a6ff;
            margin-top: 0;
            font-size: 1.5em;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        th, td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #30363d;
        }
        th {
            background-color: #161b22;
            color: #58a6ff;
        }
        tr:nth-child(even) {
            background-color: #161b22;
        }
        tr:hover {
            background-color: #1f242e;
        }
        .search-box {
            margin-bottom: 20px;
            padding: 10px;
            width: 100%;
            box-sizing: border-box;
            border: 1px solid #30363d;
            border-radius: 4px;
            background-color: #0d1117;
            color: #c9d1d9;
        }
        .code-block {
            background-color: #161b22;
            padding: 15px;
            border-radius: 6px;
            font-family: monospace;
            white-space: pre;
            overflow-x: auto;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Roblox Fast Flags</h1>
        <input type="text" id="search" class="search-box" placeholder="Search for fast flags...">
        <div id="categories">
            <div class="category">
                <h2>Dynamic Fast Flags</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Name</th>
                            <th>Value</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>DFFlagAbuseReportInExperienceStateCaptureMode</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>DFFlagAccessCookiesWithUrlEnabled</td>
                            <td>true</td>
                        </tr>
                        <!-- Add more dynamic fast flags here -->
                    </tbody>
                </table>
            </div>
            <!-- Add more categories and flags as needed -->
        </div>
    </div>
    <script>
        document.getElementById('search').addEventListener('input', function() {
            const searchTerm = this.value.toLowerCase();
            const rows = document.querySelectorAll('tbody tr');

            rows.forEach(row => {
                const name = row.querySelector('td:first-child').textContent.toLowerCase();
                if (name.includes(searchTerm)) {
                    row.style.display = '';
                } else {
                    row.style.display = 'none';
                }
            });
        });
    </script>
</body>
</html>
