<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Hai Yen - Dates in Month</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            padding-top: 50px;
            background-color: #f4f4f4;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h2 {
            text-align: center;
            margin-bottom: 20px;
            font-weight: bold;
        }
        table td {
            padding: 10px;
        }
        input, select {
            padding: 5px;
            width: 200px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        input[readonly] {
            background-color: #eee;
            font-weight: bold;
            color: #333;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>DATES IN MONTH</h2>
        <form name="f">
            <table border="0">
                <tr>
                    <td align="right">Year:</td>
                    <td>
                        <input type="text" id="year" name="year" value="2012" oninput="updateDate()">
                    </td>
                </tr>
                <tr>
                    <td align="right">Month:</td>
                    <td>
                        <select id="month" name="month" onchange="updateDate()">
                            <option value="1">01</option>
                            <option value="2">02</option>
                            <option value="3">03</option>
                            <option value="4">04</option>
                            <option value="5">05</option>
                            <option value="6">06</option>
                            <option value="7">07</option>
                            <option value="8">08</option>
                            <option value="9">09</option>
                            <option value="10">10</option>
                            <option value="11">11</option>
                            <option value="12">12</option>
                        </select>
                    </td>
                </tr>
                <tr>
                    <td align="right">Date:</td>
                    <td>
                        <input type="text" id="date" name="date" readonly>
                    </td>
                </tr>
            </table>
        </form>
    </div>

    <script>
        function isLeapYear(y) {
            return (y % 4 === 0 && y % 100 !== 0) || (y % 400 === 0);
        }

        function updateDate() {
  
            const yearVal = document.getElementById('year').value;
            const monthVal = document.getElementById('month').value;
            const dateInput = document.getElementById('date');
        }
            if (yearVal === "" || isNaN(yearVal)) {
                dateInput.value = "Year must a number";
                return; 

            const year = parseInt(yearVal);
            let days = 0;

            switch (monthVal) {
                case "1": case "3": case "5": case "7": case "8": case "10": case "12":
                    days = 31;
                    break;
                case "4": case "6": case "9": case "11":
                    days = 30;
                    break;
                case "2":
                    days = isLeapYear(year) ? 29 : 28;
                    break;
            }
            dateInput.value = days;
        }

        window.onload = updateDate;
    </script>
</body>
</html>
