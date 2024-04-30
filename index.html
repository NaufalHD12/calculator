<?php
session_start(); // Memulai sesi di awal skrip

if ($_SERVER['REQUEST_METHOD'] === 'POST' && isset($_POST['calculate'])) {
    $angka1 = $_POST['angka1'];
    $angka2 = $_POST['angka2'];
    $operator = $_POST['operator'];
    $hasil = null;

    switch($operator) {
        case '+': $hasil = $angka1 + $angka2; break;
        case '-': $hasil = $angka1 - $angka2; break;
        case '*': $hasil = $angka1 * $angka2; break;
        case '/': 
            if($angka2 != 0) {
                $hasil = $angka1 / $angka2;
            } else {
                $hasil = "Pembagian dengan nol tidak diizinkan";
            }
            break;
        default: $hasil = "Operasi tidak valid";
    }
    
    // Simpan hasil dalam sesi
    $_SESSION['hasil'] = $hasil;
    $_SESSION['angka1'] = $angka1;
    $_SESSION['angka2'] = $angka2;
    $_SESSION['operator'] = $operator;

    if (isset($hasil)) {
        echo "<div class='result'>Hasil: $angka1 $operator $angka2 = $hasil</div>";
    }

    // Redirect ke halaman ini dengan metode GET
    header('Location: ' . $_SERVER['PHP_SELF']);
    exit;
}
if ($_SERVER['REQUEST_METHOD'] === 'POST' && isset($_POST['clear'])) {
    // Hapus sesi yang menyimpan hasil dan input
    unset($_SESSION['hasil']);
    unset($_SESSION['angka1']);
    unset($_SESSION['angka2']);
    unset($_SESSION['operator']);

    // Redirect ke halaman ini dengan metode GET
    header('Location: ' . $_SERVER['PHP_SELF']);
    exit;
}
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator Sederhana</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f7f7f7;
            display: flex; /* Added for centering */
            justify-content: center; /* Added for centering */
            align-items: center; /* Added for centering */
            min-height: 100vh; /* Added for vertical centering */
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin: 0 auto; /* Removed unnecessary margin: auto */
            width: 800px;
            background: beige;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            
        }

        input, select {
            padding: 10px;
            border: 1px solid #ccc;
        }
        input[type="submit"] {
            background-color: #22c1c3;
            border: none;
            color: white;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        input[type="submit"]:hover {
            background-color: #159a9c;
        }
        input::placeholder, select {
            color: #999;
            font-style: italic;
        }
        input[type="number"]:focus, select:focus {
            outline: none;
            border: 2px solid #22c1c3;
        }
        input[type="submit"]:hover {
            transform: scale(1.05);
        }
        h1 {
            text-align: center;
            color: #333;
            font-family: 'Helvetica', sans-serif;
        }
        .result {
            text-align: center;
            margin-top: 20px;
        }

        @media (max-width: 600px) {
            form {
                width: 90%;
            }
        }

    </style>
</head>
<body>
    
    <form method="post">
        <h1>Kalkulator</h1>
        <input type="number" name="angka1" placeholder="Angka 1">
        <select name="operator">
            <option value="+">+</option>
            <option value="-">-</option>
            <option value="*">*</option>
            <option value="/">/</option>
        </select>
        <input type="number" name="angka2" placeholder="Angka 2">
        <input type="submit" name="calculate" value="Hitung 🔍">
        <input type="submit" name="clear" value="Clear" style="background-color: #f44336;"
        <!-- Tambahkan div untuk menampilkan hasil -->
        <?php if(isset($_SESSION['hasil'])): ?>
        <div class="result">
            <?php
                // Tampilkan hasil dari sesi
                echo "Hasil: " . $_SESSION['angka1'] . " " . $_SESSION['operator'] . " " . $_SESSION['angka2'] . " = " . $_SESSION['hasil'];
            ?>
        </div>
        <?php endif; ?>
    </form>
    
</body>
</html>
