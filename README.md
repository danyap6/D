<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pembayaran</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .payment-method {
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <h1>Pembayaran</h1>
    <form>
        <div class="payment-method">
            <input type="radio" id="dana" name="payment-method" value="dana">
            <label for="dana">Dana</label>
        </div>
        <div class="payment-method">
            <input type="radio" id="ovo" name="payment-method" value="ovo">
            <label for="ovo">OVO</label>
        </div>
        <div class="payment-method">
            <input type="radio" id="gopay" name="payment-method" value="gopay">
            <label for="gopay">GoPay</label>
        </div>
        <div class="payment-method">
            <input type="radio" id="qris" name="payment-method" value="qris">
            <label for="qris">QRIS</label>
        </div>
        <button type="submit">Bayar</button>
    </form>

    <!-- Contoh script untuk menangani pembayaran -->
    <script>
        const form = document.querySelector('form');
        form.addEventListener('submit', (e) => {
            e.preventDefault();
            const paymentMethod = document.querySelector('input[name="payment-method"]:checked').value;
            // Lakukan sesuatu dengan paymentMethod, seperti mengirim request ke server untuk memproses pembayaran
            console.log(paymentMethod);
        });
    </script>
</body>
</html>
