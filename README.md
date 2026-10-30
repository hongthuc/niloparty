<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NILO Cakes & Decor - niloparty.com</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Inter & FontAwesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        nilo: {
                            50: '#fdf2f4',
                            100: '#fbe8ec',
                            500: '#e11d48',
                            600: '#be123c',
                            700: '#9f1239',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body { font-family: 'Inter', sans-serif; }
        .flatsome-shadow { box-shadow: 0 2px 10px rgba(0,0,0,0.06); }
        .card-hover:hover { transform: translateY(-3px); transition: all 0.3s ease; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 antialiased">

    <!-- Top Bar (Clean, no UX builder editor text) -->
    <div class="bg-gray-900 text-gray-300 text-xs py-2 px-4">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-1">
            <div class="flex items-center gap-4">
                <span><i class="fa-solid fa-location-dot text-nilo-500 mr-1"></i> 12 Phú Lộc 3, Thanh Khê, Đà Nẵng</span>
                <span class="hidden md:inline"><i class="fa-solid fa-clock text-nilo-500 mr-1"></i> 8:00 - 21:00 (T2 - CN)</span>
            </div>
            <div class="flex items-center gap-4">
                <a href="tel:0905400344" class="hover:text-white"><i class="fa-solid fa-phone text-nilo-500 mr-1"></i> 0905.400.344</a>
                <span>-</span>
                <a href="tel:0377794379" class="hover:text-white">0377.794.379</a>
            </div>
        </div>
    </div>

    <!-- Header Section (Flatsome Style Header) -->
    <header class="bg-white border-b border-gray-200 sticky top-0 z-40 flatsome-shadow">
        <div class="max-w-7xl mx-auto px-4 py-3 flex items-center justify-between gap-4">
            <!-- Mobile Menu Button -->
            <button class="md:hidden text-gray-700 text-xl focus:outline-none" onclick="toggleMobileMenu()">
                <i class="fa-solid fa-bars"></i>
            </button>

            <!-- Logo -->
            <div class="flex items-center gap-2">
                <a href="#" class="flex items-center gap-2">
                    <div class="bg-nilo-500 text-white font-bold rounded-lg p-2 text-xl flex items-center justify-center w-10 h-10 shadow">
                        N
                    </div>
                    <div>
                        <span class="text-xl font-bold tracking-tight text-gray-900 block leading-tight">NILO CAKES & DECOR</span>
                        <span class="text-xs text-nilo-600 font-semibold uppercase tracking-wider">niloparty.com</span>
                    </div>
                </a>
            </div>

            <!-- Search Bar (Desktop) -->
            <div class="hidden md:flex flex-1 max-w-lg mx-6">
                <div class="relative w-full">
                    <input type="text" placeholder="Tìm kiếm mẫu trang trí, bóng bay, bánh kem..." class="w-full bg-gray-100 border border-gray-300 rounded-l-md px-4 py-2 text-sm focus:outline-none focus:border-nilo-500">
                    <button class="absolute right-0 top-0 bottom-0 bg-nilo-500 text-white px-5 rounded-r-md hover:bg-nilo-600 transition">
                        <i class="fa-solid fa-search"></i>
                    </button>
                </div>
            </div>

            <!-- Right Actions -->
            <div class="flex items-center gap-4">
                <a href="https://zalo.me/0905400344" target="_blank" class="hidden sm:flex items-center gap-1 bg-blue-50 text-blue-600 px-3 py-1.5 rounded-full text-xs font-medium hover:bg-blue-100 transition">
                    <i class="fa-solid fa-comment-sms"></i> Zalo Chat
                </a>
                <a href="https://www.facebook.com/nilodecor.danang" target="_blank" class="flex items-center gap-1 bg-nilo-50 text-nilo-600 px-3 py-1.5 rounded-full text-xs font-medium hover:bg-nilo-100 transition">
                    <i class="fa-brands fa-facebook"></i> Fanpage
                </a>
            </div>
        </div>

        <!-- Navigation Menu Bar -->
        <nav class="bg-white border-t border-gray-100 hidden md:block">
            <div class="max-w-7xl mx-auto px-4 flex items-center justify-between">
                <ul class="flex space-x-8 text-sm font-medium py-3">
                    <li><a href="#" class="text-nilo-600 font-semibold hover:text-nilo-700">Trang Chủ</a></li>
                    <li><a href="#danhmuc" class="text-gray-700 hover:text-nilo-600 transition">Danh Mục Sản Phẩm <i class="fa-solid fa-chevron-down text-xs ml-1"></i></a></li>
                    <li><a href="#trangtri" class="text-gray-700 hover:text-nilo-600 transition">Trang Trí Sinh Nhật</a></li>
                    <li><a href="#setdecor" class="text-gray-700 hover:text-nilo-600 transition">Set Tự Decor</a></li>
                    <li><a href="#diachi" class="text-gray-700 hover:text-nilo-600 transition">Liên Hệ & Bản Đồ</a></li>
                </ul>
                <div class="text-xs text-gray-500 font-medium">
                    Hotline: <span class="text-nilo-600 font-bold">0905.400.344</span>
                </div>
            </div>
        </nav>

        <!-- Mobile Menu Drawer (Hidden by default) -->
        <div id="mobileMenu" class="hidden md:hidden bg-white border-b border-gray-200 px-4 pt-2 pb-4 space-y-2">
            <a href="#" class="block py-2 text-nilo-600 font-semibold border-b border-gray-100">Trang Chủ</a>
            <a href="#danhmuc" class="block py-2 text-gray-700 border-b border-gray-100">Danh Mục Sản Phẩm</a>
            <a href="#trangtri" class="block py-2 text-gray-700 border-b border-gray-100">Trang Trí Sinh Nhật</a>
            <a href="#setdecor" class="block py-2 text-gray-700 border-b border-gray-100">Set Tự Decor</a>
            <a href="#diachi" class="block py-2 text-gray-700">Liên Hệ & Bản Đồ</a>
        </div>
    </header>

    <!-- Hero Banner Section -->
    <section class="relative bg-gradient-to-r from-rose-900 to-nilo-700 text-white py-12 md:py-20 px-4 overflow-hidden">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8 items-center relative z-10">
            <div class="space-y-4">
                <span class="bg-white/20 text-white text-xs font-semibold px-3 py-1 rounded-full uppercase tracking-wider">NILO Cakes & Decor Đà Nẵng</span>
                <h1 class="text-3xl md:text-5xl font-extrabold tracking-tight leading-tight">Trang Trí Tiệc & Sự Kiện Chuyên Nghiệp</h1>
                <p class="text-rose-100 text-sm md:text-base leading-relaxed">Chuyên trang trí sinh nhật, thôi nôi, khai trương, set tự decor tại nhà và các mẫu bánh kem thiết kế riêng ấn tượng tại Đà Nẵng.</p>
                <div class="flex flex-wrap gap-3 pt-2">
                    <a href="tel:0905400344" class="bg-white text-nilo-700 font-semibold px-6 py-3 rounded-md shadow hover:bg-rose-50 transition text-sm">
                        <i class="fa-solid fa-phone mr-2"></i> Tư Vấn Nhanh
                    </a>
                    <a href="https://www.facebook.com/nilodecor.danang" target="_blank" class="border border-white/40 hover:bg-white/10 text-white font-semibold px-6 py-3 rounded-md transition text-sm">
                        Xem Mẫu Trên Fanpage
                    </a>
                </div>
            </div>
            <div class="hidden md:block">
                <div class="bg-white/10 backdrop-blur-md p-4 rounded-xl border border-white/20 shadow-xl">
                    <img src="https://placehold.co/600x400/be123c/ffffff?text=NILO+Party+Decor" alt="NILO Decor" class="rounded-lg w-full h-auto object-cover">
                </div>
            </div>
        </div>
    </section>

    <!-- Categories Section (Optimized for Desktop & Mobile) -->
    <section id="danhmuc" class="max-w-7xl mx-auto px-4 py-12">
        <div class="text-center mb-10">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-900">Danh Mục Sản Phẩm & Dịch Vụ</h2>
            <p class="text-gray-500 text-sm mt-1">Lựa chọn các dịch vụ và phụ kiện trang trí tiệc theo chủ đề</p>
        </div>

        <!-- Categories Grid -->
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4">
            <!-- Cat 1 -->
            <a href="#trangtri" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-cake-candles text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">Sinh Nhật Bé Trai</h3>
                <span class="text-xs text-gray-400 mt-1 block">Backdrop, Chipi</span>
            </a>
            <!-- Cat 2 -->
            <a href="#trangtri" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-gift text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">Sinh Nhật Bé Gái</h3>
                <span class="text-xs text-gray-400 mt-1 block">Công chúa, Pastel</span>
            </a>
            <!-- Cat 3 -->
            <a href="#trangtri" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-store text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">Khai Trương</h3>
                <span class="text-xs text-gray-400 mt-1 block">Kệ hoa, Bóng bay</span>
            </a>
            <!-- Cat 4 -->
            <a href="#setdecor" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-box-open text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">Set Tự Decor</h3>
                <span class="text-xs text-gray-400 mt-1 block">Tiện lợi, Giá tốt</span>
            </a>
            <!-- Cat 5 -->
            <a href="#danhmuc" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-icons text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">Phụ Kiện & Chipi</h3>
                <span class="text-xs text-gray-400 mt-1 block">Hashtag, Nón</span>
            </a>
            <!-- Cat 6 -->
            <a href="#danhmuc" class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center card-hover group">
                <div class="w-16 h-16 mx-auto mb-3 bg-rose-50 rounded-full flex items-center justify-center text-nilo-500 group-hover:bg-nilo-500 group-hover:text-white transition">
                    <i class="fa-solid fa-file-pen text-2xl"></i>
                </div>
                <h3 class="font-semibold text-sm text-gray-800">File Thiết Kế</h3>
                <span class="text-xs text-gray-400 mt-1 block">Vector, Backdrop</span>
            </a>
        </div>
    </section>

    <!-- Product Section (2 Columns on Mobile, 4 Columns on Desktop as requested) -->
    <section id="trangtri" class="max-w-7xl mx-auto px-4 py-8">
        <div class="flex justify-between items-end mb-6">
            <div>
                <span class="text-nilo-600 font-semibold text-xs uppercase tracking-wider">Mẫu Hot 2026</span>
                <h2 class="text-2xl font-bold text-gray-900">Sản Phẩm & Gói Trang Trí Nổi Bật</h2>
            </div>
            <a href="https://www.facebook.com/nilodecor.danang" target="_blank" class="text-sm font-semibold text-nilo-600 hover:underline hidden sm:block">Xem tất cả trên Fanpage <i class="fa-solid fa-arrow-right ml-1"></i></a>
        </div>

        <!-- Product Grid: grid-cols-2 on mobile, md:grid-cols-4 on desktop -->
        <div class="grid grid-cols-2 md:grid-cols-4 gap-3 md:gap-6">
            <!-- Product 1 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="relative overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://placehold.co/400x400/f3f4f6/be123c?text=Backdrop+Safari" alt="Safari Pastel" class="w-full h-full object-cover">
                        <span class="absolute top-2 left-2 bg-nilo-500 text-white text-[10px] font-bold px-2 py-0.5 rounded">HOT</span>
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Trang Trí Sinh Nhật</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Safari Pastel Sang Trọng (4m x 2m4)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-medium px-3 py-1.5 rounded transition">Đặt lịch</a>
                </div>
            </div>

            <!-- Product 2 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="relative overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://placehold.co/400x400/f3f4f6/be123c?text=Gau+Phi+Cong" alt="Gấu Phi Công" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Trai</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Wilson - Gấu Phi Công Baby (2m4 x 2m)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-medium px-3 py-1.5 rounded transition">Đặt lịch</a>
                </div>
            </div>

            <!-- Product 3 -->
            <div id="setdecor" class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="relative overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://placehold.co/400x400/f3f4f6/be123c?text=Set+Sinh+Nhat+499K" alt="Set Sinh Nhật" class="w-full h-full object-cover">
                        <span class="absolute top-2 left-2 bg-blue-600 text-white text-[10px] font-bold px-2 py-0.5 rounded">TỰ DECOR</span>
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Set Sinh Nhật</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Set Sinh Nhật Tự Decor Theo Tên Bé (Ship Toàn Quốc)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">499.000đ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-medium px-3 py-1.5 rounded transition">Mua ngay</a>
                </div>
            </div>

            <!-- Product 4 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="relative overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://placehold.co/400x400/f3f4f6/be123c?text=Khai+Truong+Shop" alt="Khai Trương" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Khai Trương</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Backdrop Khai Trương Tấm Boutique - Tone Nâu Kem</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-medium px-3 py-1.5 rounded transition">Đặt lịch</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Address & Map Section (Map image/embed out to homepage) -->
    <section id="diachi" class="max-w-7xl mx-auto px-4 py-12">
        <div class="bg-white rounded-2xl shadow-sm border border-gray-200 overflow-hidden grid grid-cols-1 md:grid-cols-2">
            <div class="p-6 md:p-10 flex flex-col justify-center space-y-4">
                <span class="text-nilo-600 font-semibold text-xs uppercase tracking-wider">Thông Tin Liên Hệ</span>
                <h2 class="text-2xl md:text-3xl font-bold text-gray-900">NILO Cakes & Decor Đà Nẵng</h2>
                <p class="text-gray-600 text-sm">Cửa hàng chuyên cung cấp dịch vụ trang trí tiệc sinh nhật, thôi nôi, sự kiện và các mẫu bánh kem đẹp mắt tại Đà Nẵng.</p>
                
                <div class="space-y-3 pt-2 text-sm">
                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-location-dot"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Địa chỉ cửa hàng:</span>
                            <span class="text-gray-600">12 Phú Lộc 3, Thanh Khê, Đà Nẵng</span>
                        </div>
                    </div>
                    
                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Hotline / Zalo:</span>
                            <span class="text-gray-600">0905.400.344 - 0377.794.379</span>
                        </div>
                    </div>

                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-globe"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Website & Fanpage:</span>
                            <span class="text-gray-600">niloparty.com | fb.com/nilodecor.danang</span>
                        </div>
                    </div>
                </div>

                <div class="pt-2 flex gap-3">
                    <a href="https://maps.app.goo.gl/e5YRjwo3E7bB7oao6" target="_blank" class="bg-nilo-500 hover:bg-nilo-600 text-white px-5 py-2.5 rounded-md text-sm font-semibold transition shadow-sm">
                        <i class="fa-solid fa-map-location-dot mr-2"></i> Mở Google Maps
                    </a>
                </div>
            </div>

            <!-- Map View / Map Image Preview on Homepage -->
            <div class="relative bg-gray-100 min-h-[300px] flex items-center justify-center p-4">
                <div class="w-full h-full rounded-xl overflow-hidden shadow-inner border border-gray-200 flex flex-col items-center justify-center bg-rose-50 p-6 text-center">
                    <div class="w-16 h-16 bg-nilo-500 text-white rounded-full flex items-center justify-center text-2xl shadow mb-4 animate-bounce">
                        <i class="fa-solid fa-map-pin"></i>
                    </div>
                    <h3 class="font-bold text-lg text-gray-900 mb-1">12 Phú Lộc 3, Thanh Khê, Đà Nẵng</h3>
                    <p class="text-xs text-gray-500 mb-4">Nhấn vào bên dưới để xem đường đi chi tiết qua Google Maps</p>
                    <a href="https://maps.app.goo.gl/e5YRjwo3E7bB7oao6" target="_blank" class="bg-white border border-nilo-500 text-nilo-600 hover:bg-nilo-500 hover:text-white px-4 py-2 rounded-lg text-xs font-bold transition shadow-sm">
                        Xem bản đồ trực tuyến <i class="fa-solid fa-arrow-right ml-1"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-gray-900 text-gray-400 py-10 px-4 mt-12 text-sm">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 mb-8">
            <div>
                <h3 class="text-white font-bold text-base mb-3">NILO Cakes & Decor</h3>
                <p class="text-xs leading-relaxed text-gray-400">Chuyên cung cấp dịch vụ trang trí tiệc sinh nhật, thôi nôi, khai trương và các set phụ kiện tự decor chất lượng cao tại Đà Nẵng.</p>
            </div>
            <div>
                <h3 class="text-white font-bold text-base mb-3">Danh Mục Chính</h3>
                <ul class="space-y-2 text-xs">
                    <li><a href="#trangtri" class="hover:text-white transition">Trang trí sinh nhật bé trai / bé gái</a></li>
                    <li><a href="#trangtri" class="hover:text-white transition">Trang trí khai trương cửa hàng</a></li>
                    <li><a href="#setdecor" class="hover:text-white transition">Set sinh nhật tự decor tại nhà</a></li>
                    <li><a href="#danhmuc" class="hover:text-white transition">Phụ kiện & Chipi thiết kế</a></li>
                </ul>
            </div>
            <div>
                <h3 class="text-white font-bold text-base mb-3">Kết Nối Với Chúng Tôi</h3>
                <p class="text-xs mb-3">Hotline tư vấn nhanh: <strong class="text-white">0905.400.344</strong></p>
                <div class="flex gap-3">
                    <a href="https://www.facebook.com/nilodecor.danang" target="_blank" class="w-9 h-9 bg-blue-600 text-white rounded-full flex items-center justify-center hover:bg-blue-700 transition"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="https://zalo.me/0905400344" target="_blank" class="w-9 h-9 bg-sky-500 text-white rounded-full flex items-center justify-center hover:bg-sky-600 transition"><i class="fa-solid fa-comment"></i></a>
                </div>
            </div>
        </div>
        <div class="max-w-7xl mx-auto border-t border-gray-800 pt-6 text-center text-xs text-gray-500">
            <p>&copy; 2026 niloparty.com - NILO Cakes & Decor. All rights reserved.</p>
        </div>
    </footer>

    <!-- Floating Contact Buttons (Zalo & Facebook) -->
    <div class="fixed bottom-6 right-6 z-50 flex flex-col gap-3">
        <!-- Zalo Button -->
        <a href="https://zalo.me/0905400344" target="_blank" title="Chat Zalo" class="w-12 h-12 bg-sky-500 text-white rounded-full shadow-lg flex items-center justify-center text-xl hover:bg-sky-600 transition transform hover:scale-110">
            <i class="fa-solid fa-comment-dots"></i>
        </a>
        <!-- Facebook Messenger Button -->
        <a href="https://www.facebook.com/nilodecor.danang" target="_blank" title="Chat Facebook" class="w-12 h-12 bg-blue-600 text-white rounded-full shadow-lg flex items-center justify-center text-xl hover:bg-blue-700 transition transform hover:scale-110">
            <i class="fa-brands fa-facebook-messenger"></i>
        </a>
    </div>

    <!-- Script to toggle mobile menu -->
    <script>
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
            } else {
                menu.classList.add('hidden');
            }
        }
    </script>
</body>
</html>
