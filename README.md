<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>F.T. BEAUTY AND WELLNESS CO., LTD. </title>
    <style>
        /* กำหนดสีหลักและพื้นหลัง */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            background-color: #f0f8ff; /* สีฟ้าอ่อน */
            color: #003366; /* สีน้ำเงินเข้ม */
        }
        .header {
            display: flex;
            align-items: center;
            padding: 10px;
            background-color: #005b96; /* สีน้ำเงิน */
            color: white;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        .header img {
            width: 80px;
            margin-right: 15px;
            border-radius: 50%;
            border: 2px solid white;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }

        .button-container {
            display: flex;
            justify-content: flex-end; /* วางปุ่มด้านขวา */
            align-items: center;
            margin-bottom: 20px;
        }
        .sup-dropdown {
            padding: 10px;
            margin-right: 10px;
            border: 1px solid #b0c4de;
            border-radius: 5px;
            background-color: #ffffff;
            color: #003366;
            font-weight: bold;
        }
        .transfer-button {
            padding: 10px 15px;
            background-color: #007BFF; /* สีฟ้า */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        .transfer-button:hover {
            background-color: #0056b3; /* สีเข้มเมื่อ hover */
        }

        form {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        label {
            display: block;
            margin: 10px 0 5px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #b0c4de;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input:read-only {
            background-color: #e6f2ff;
        }
        .submit-button {
            width: 100%;
            padding: 10px;
            background-color: #005b96;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        .submit-button:hover {
            background-color: #004080;
        }
    </style>
</head>
<body>
    <div class="header">
        <a href="https://example.com">
            <img src="https://i.imgur.com/baPKb6z.jpg" alt="โลโก้หรือชื่อบริษัท">
        </a>
        <h1>WS_Sup P' Tuche เบิกสินค้า 2024</h1>
    </div>

    <div class="button-container">
        <select id="supSelect" class="sup-dropdown">
            <option value="">-- เลือก Sup --</option>
            <option value="Sup Nina">Sup Nina</option>
            <option value="Sup Tuche">Sup Tuche</option>
            <option value="Sup Aum">Sup Aum</option>
            <option value="Sup Manow">Sup Manow</option>
            <option value="Sup Whan">Sup Whan</option>
            <option value="Sup Ming">Sup Ming</option>
        </select>
        <button type="button" class="transfer-button" onclick="transferItem()">โอนย้าย</button>
    </div>

    <form id="productForm">
        <label for="date">วันที่:</label>
        <input type="date" id="date" required>

        <label for="branch">ชื่อสาขา:</label>
        <select id="branch" required>
            <option value="">-- เลือกสาขา --</option>
            <option value="217">217 มาบุญครอง 1</option>
            <option value="363">363 มีนบุรี</option>
            <option value="379">379 เซ็นทรัล พัทยา บีช ชั้น 3</option>
            <option value="395">395 ฮาร์เบอร์มอลล์แหลมฉบัง</option>
            <option value="400">400 ซีคอน สแควร์ 1</option>
            <option value="435">435 เซ็นทรัลลาดพร้าว</option>
            <option value="467">467 บิ๊กซี พัทยากลาง</option>
            <option value="470">470 เมก้า บางนา 1</option>
            <option value="477">477 โลตัส ศรีนครินทร์</option>
            <option value="593">593 เดอะ พาสิโอ พาร์ค</option>
            <option value="646">646 เซ็นทรัล ปิ่นเกล้า</option>
            <option value="684">684 เซ็นทรัลมารีนา</option>
            <option value="695">695 โลตัส สุขาภิบาล 3</option>
            <option value="734">734 โลตัส บ่อวิน</option>
            <option value="735">735 โลตัส ปทุมธานี</option>
            <option value="799">799 โลตัส กำแพงแสน</option>
            <option value="814">814 เทอมินอล 21 พัทยา</option>
            <option value="960">960 อิมพีเรียล เวิล์ด สำโรง ชั้น 2</option>
            <option value="3005">3005 เซ็นทรัล พัทยา บีช ชั้นจี</option>
            <option value="3006">3006 โรบินสัน บ่อวิน</option>
            <option value="3012">3012 บิ๊กซี พัทยาใต้</option>
            <option value="3053">3053 อิมพีเรียล เวิล์ด สำโรง ชั้น GF</option>
            <option value="245">245 โลตัส สุขุมวิท 50</option>
            <option value="567">567 โรบินสัน สุขุมวิท</option>
            <option value="3180">3180 บิ๊กซี รัชดา</option>
            <option value="3213">3213 เซ็นจูรี่ สุขุมวิท</option>
            <option value="762">762 เซ็นทรัล มหาชัย</option>
            <option value="632">632 เซ็นทรัล อีสวิลล์</option>
            <option value="480">480 ซีคอนสแควร์2</option>
        </select>

        <label for="productCode">รหัสสินค้า:</label>
        <select id="productCode" required onchange="updateProductDetails()">
            <option value="">-- เลือกรหัสสินค้า --</option>
            <option value="RDPT-01">RDPT-01: Derma J โทนเนอร์ 140ml.</option>
            <option value="RDPC-01">RDPC-01: Derma J ครีม 50ml.</option>
            <option value="RDPM-01">RDPM-01: Derma J มาส์กกล่อง 35g.x5</option>
            <option value="RDSC-01">RDSC-01: Derma J กันแดด 50ml.</option>
            <option value="RDPM-02">RDPM-02: Derma J มาส์กแผ่น 35g.x1</option>
            <option value="RDFC-01">RDFC-01: Derma J โฟม 140ml.</option>
            <option value="HL11A">HL11A: Herbalist คลีนซิ่ง 100ml.</option>
            <option value="HL21A">HL21A: Herbalist โฟม 100ml.</option>
            <option value="HL31A">HL31A: Herbalist เจล 35g.</option>
            <option value="HL41A">HL41A: Herbalist กันแดด 30g.</option>
            <option value="HL51A">HL51A: Herbalist ยูธ เซรั่ม 30ml.</option>
            <option value="HL61A">HL61A: Herbalist โอเวอร์ไนท์ มาส์ค 50ml.</option>
            <option value="HL32A">HL32A: Herbalist แอรี่ เจล 50g.</option>

```html
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ระบบจัดการสินค้า</title>
    <style>
        /* กำหนดสีหลักและพื้นหลัง */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            background-color: #f0f8ff; /* สีฟ้าอ่อน */
            color: #003366; /* สีน้ำเงินเข้ม */
        }
        .header {
            display: flex;
            align-items: center;
            padding: 10px;
            background-color: #005b96; /* สีน้ำเงิน */
            color: white;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        .header img {
            width: 80px;
            margin-right: 15px;
            border-radius: 50%;
            border: 2px solid white;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }

        .button-container {
            display: flex;
            justify-content: flex-end; /* วางปุ่มด้านขวา */
            align-items: center;
            margin-bottom: 20px;
        }
        .sup-dropdown {
            padding: 10px;
            margin-right: 10px;
            border: 1px solid #b0c4de;
            border-radius: 5px;
            background-color: #ffffff;
            color: #003366;
            font-weight: bold;
        }
        .transfer-button {
            padding: 10px 15px;
            background-color: #007BFF; /* สีฟ้า */
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        .transfer-button:hover {
            background-color: #0056b3; /* สีเข้มเมื่อ hover */
        }

        form {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        label {
            display: block;
            margin: 10px 0 5px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #b0c4de;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input:read-only {
            background-color: #e6f2ff;
        }
        .submit-button {
            width: 100%;
            padding: 10px;
            background-color: #005b96;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        .submit-button:hover {
            background-color: #004080;
        }
    </style>
</head>
<body>
    <div class="header">
        <a href="https://example.com">
            <img src="https://i.imgur.com/baPKb6z.jpg" alt="โลโก้หรือชื่อบริษัท">
        </a>
        <h1>ระบบจัดการสินค้า</h1>
    </div>



        <label for="status">สถานะสินค้า:</label>
        <input type="text" id="status" value="ปกติ" readonly>

        <label for="currentStock">คงเหลือปัจจุบัน:</label>
        <input type="number" id="currentStock" readonly>

        <label for="withdraw">จำนวนเบิก:</label>
        <input type="number" id="withdraw" required>

        <label for="sendActual">จำนวนส่งจริง:</label>
        <input type="number" id="" required oninput="calculateTotal()">

        <label for="total">รวม:</label>
        <input type="number" id="total" readonly>

        <button type="submit" class="submit-button">บันทึกข้อมูล</button>
    </form>

    <script>
        const productDetails = {
            "RDPT-01": { status: "สินค้าหมด", currentStock: 6 },
            "RDPC-01": { status: "ขายดี", currentStock: 80 },
            "RDPM-01": { status: "ขาย", currentStock: 50 },
            "RDSC-01": { status: "พร้อมขาย", currentStock: 200 },
            "RDPM-02": { status: "ขาย", currentStock: 150 },
            "RDFC-01": { status: "พร้อมขาย", currentStock: 100 },
            "HL11A": { status: "พร้อมขาย", currentStock: 60 },
            "HL21A": { status: "ขายดี", currentStock: 90 },
            "HL31A": { status: "ขาย", currentStock: 20 },
            "HL41A": { status: "พร้อมขาย", currentStock: 300 },
            "HL51A": { status: "ขาย", currentStock: 0 },
            "HL61A": { status: "ขายดี", currentStock: 10 },
            "HL32A": { status: "พร้อมขาย", currentStock: 45 },
            "HL71A": { status: "พร้อมขาย", currentStock: 80 },
            "HL42A": { status: "ขาย", currentStock: 30 },
            "HL81A": { status: "ขายดี", currentStock: 5 },
            "HL52A": { status: "พร้อมขาย", currentStock: 75 },
            "EC-01A": { status: "พร้อมขาย", currentStock: 50 },
            "ES-01": { status: "ขายดี", currentStock: 40 },
        };

        function updateProductDetails() {
            const productCode = document.getElementById("productCode").value;
            const statusInput = document.getElementById("status");
            const currentStockInput = document.getElementById("currentStock");

            if (productCode in productDetails) {
                const details = productDetails[productCode];
                statusInput.value = details.status;
                currentStockInput.value = details.currentStock;
                calculateTotal();
            } else {
                statusInput.value = "";
                currentStockInput.value = "";
            }
        }

        function calculateTotal() {
            const withdrawInput = document.getElementById("withdraw").value;
            const sendActualInput = document.getElementById("sendActual").value;
            const totalInput = document.getElementById("total");

            const currentStock = parseInt(document.getElementById("currentStock").value);
            const withdraw = parseInt(withdrawInput) || 0;
            const sendActual = parseInt(sendActualInput) || 0;

            if (withdraw + sendActual <= currentStock) {
                totalInput.value = withdraw + sendActual;
            } else {
                alert("จำนวนเบิกและส่งจริงต้องไม่เกินคงเหลือปัจจุบัน");
                totalInput.value = "";
            }
        }

        function transferItem() {
            const selectedSup = document.getElementById("supSelect").value;
            if (selectedSup) {
                alert('โอนย้ายสินค้าไปยัง ' + selectedSup + ' สำเร็จ');
            } else {
                alert('กรุณาเลือกชื่อ Sup ก่อนโอนย้ายสินค้า');
            }
        }

        document.getElementById("productForm").addEventListener("submit", function(event) {
            event.preventDefault();
            alert("บันทึกข้อมูลเรียบร้อยแล้ว");
            this.reset();
            document.getElementById("total").value = ""; // Reset total field
        });
    </script>
</body>
</html>
