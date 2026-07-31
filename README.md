<!DOCTYPE html>
<html lang="az">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sip & Fresh — İçki Menyusu</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-amber-50 text-gray-800 font-sans pb-10">

    <!-- Header -->
    <header class="bg-orange-500 text-white p-5 shadow-lg flex justify-between items-center sticky top-0 z-10">
        <h1 class="text-2xl font-bold flex items-center gap-2">🍹 Sip & Fresh</h1>
        <div class="bg-orange-600 px-4 py-2 rounded-full text-sm font-semibold">
            🛒 Səbət: <span id="cart-count">0</span> məhsul
        </div>
    </header>

    <!-- Qarşılama -->
    <div class="text-center my-8 px-4">
        <h2 class="text-3xl font-extrabold text-orange-600 mb-2">Təzə Şirələr və Qəhvələr</h2>
        <p class="text-gray-600">Sevdiyiniz içkini seçin və sifariş simulyasiyasını sınayın!</p>
    </div>

    <!-- Məhsullar Şəbəkəsi (Grid) -->
    <main class="max-w-6xl mx-auto grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 px-4">

        <!-- Məhsul 1: Portaqal Şirəsi -->
        <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition flex flex-col justify-between">
            <img src="https://images.unsplash.com/photo-1613478223719-2ab802602423?w=500" alt="Portaqal Şirəsi" class="h-48 w-full object-cover">
            <div class="p-5 flex-1 flex flex-col justify-between">
                <div>
                    <h3 class="text-xl font-bold">100% Portaqal Şirəsi</h3>
                    <p class="text-gray-500 text-sm mt-1">Təzə sıxılmış təbii C vitamini deposu.</p>
                </div>
                <div class="flex justify-between items-center mt-4 pt-3 border-t">
                    <span class="text-lg font-bold text-orange-600">4.50 AZN</span>
                    <button onclick="addToCart()" class="bg-orange-500 text-white px-4 py-2 rounded-xl hover:bg-orange-600 transition">Səbətə At</button>
                </div>
            </div>
        </div>

        <!-- Məhsul 2: Qapuçino -->
        <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition flex flex-col justify-between">
            <img src="https://images.unsplash.com/photo-1572442388796-11668a67e53d?w=500" alt="Cappuccino" class="h-48 w-full object-cover">
            <div class="p-5 flex-1 flex flex-col justify-between">
                <div>
                    <h3 class="text-xl font-bold">Klassik Cappuccino</h3>
                    <p class="text-gray-500 text-sm mt-1">Zərif südlü köpük və zəngin espresso dadı.</p>
                </div>
                <div class="flex justify-between items-center mt-4 pt-3 border-t">
                    <span class="text-lg font-bold text-orange-600">5.00 AZN</span>
                    <button onclick="addToCart()" class="bg-orange-500 text-white px-4 py-2 rounded-xl hover:bg-orange-600 transition">Səbətə At</button>
                </div>
            </div>
        </div>

        <!-- Məhsul 3: Detoks Miks -->
        <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition flex flex-col justify-between">
            <img src="https://images.unsplash.com/photo-1622597467836-f3285f2131b7?w=500" alt="Detoks Sok" class="h-48 w-full object-cover">
            <div class="p-5 flex-1 flex flex-col justify-between">
                <div>
                    <h3 class="text-xl font-bold">Yaşıl Detoks Miks</h3>
                    <p class="text-gray-500 text-sm mt-1">Xiyar, yaşıl alma və nane qarışığı.</p>
                </div>
                <div class="flex justify-between items-center mt-4 pt-3 border-t">
                    <span class="text-lg font-bold text-orange-600">6.00 AZN</span>
                    <button onclick="addToCart()" class="bg-orange-500 text-white px-4 py-2 rounded-xl hover:bg-orange-600 transition">Səbətə At</button>
                </div>
            </div>
        </div>

        <!-- Məhsul 4: İce Latte -->
        <div class="bg-white rounded-2xl shadow-md overflow-hidden hover:shadow-xl transition flex flex-col justify-between">
            <img src="https://images.unsplash.com/photo-1517701604599-bb29b565090c?w=500" alt="Iced Latte" class="h-48 w-full object-cover">
            <div class="p-5 flex-1 flex flex-col justify-between">
                <div>
                    <h3 class="text-xl font-bold">Soyuq Iced Latte</h3>
                    <p class="text-gray-500 text-sm mt-1">Yaz və yay günləri üçün sərinlədici qəhvə.</p>
                </div>
                <div class="flex justify-between items-center mt-4 pt-3 border-t">
                    <span class="text-lg font-bold text-orange-600">5.50 AZN</span>
                    <button onclick="addToCart()" class="bg-orange-500 text-white px-4 py-2 rounded-xl hover:bg-orange-600 transition">Səbətə At</button>
                </div>
            </div>
        </div>

    </main>

    <script>
        let count = 0;
        function addToCart() {
            count++;
            document.getElementById('cart-count').innerText = count;
            alert('Məhsul səbətə əlavə olundu!');
        }
    </script>
</body>
</html>

- 
