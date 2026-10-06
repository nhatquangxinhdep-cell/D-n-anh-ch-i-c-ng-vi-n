<!DOCTYPE html>
<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đêm Hội Nhạc Dân Tộc - Âm Sắc Quê Hương</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Playfair Display & Be Vietnam Pro -->
    <link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,500;0,700;0,900;1,400&display=swap" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        indochineRed: '#800020',
                        indochineGold: '#D4AF37',
                        indochineDark: '#2C1D1A',
                        indochineCream: '#FDFBF7',
                        indochineGreen: '#1E4620',
                    },
                    fontFamily: {
                        serif: ['"Playfair Display"', 'serif'],
                        sans: ['"Be Vietnam Pro"', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Be Vietnam Pro', sans-serif;
            background-color: #FDFBF7;
            color: #2C1D1A;
        }
        .font-serif {
            font-family: 'Playfair Display', serif;
        }
        /* Họa tiết trống đồng ẩn background */
        .bg-dong-son {
            background-image: radial-gradient(circle, rgba(212,175,55,0.08) 0%, rgba(128,0,32,0.03) 100%);
        }
        .text-gold-gradient {
            background: linear-gradient(135deg, #BF953F, #FCF6BA, #B38728, #FBF5B7, #AA771C);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .border-gold-glow {
            border-color: #D4AF37;
            box-shadow: 0 0 15px rgba(212, 175, 55, 0.2);
        }
    </style>
</head>
<body class="bg-dong-son min-h-screen flex flex-col selection:bg-indochineGold selection:text-white">

    <header class="sticky top-0 z-50 bg-indochineDark/95 backdrop-blur-md border-b border-indochineGold/30 text-indochineCream">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 rounded-full border border-indochineGold flex items-center justify-center bg-indochineRed">
                    <i class="fas fa-music text-indochineGold"></i>
                </div>
                <div>
                    <span class="font-serif text-lg font-bold text-indochineGold tracking-wide">HỒN VIỆT</span>
                    <p class="text-xs text-gray-300">Đêm Hội Nhạc Dân Tộc</p>
                </div>
            </div>
            <nav class="hidden md:flex space-x-8 text-sm font-medium">
                <a href="#about" class="hover:text-indochineGold transition">Giới Thiệu</a>
                <a href="#host" class="hover:text-indochineGold transition">Chủ Trì Sân Khấu</a>
                <a href="#program" class="hover:text-indochineGold transition">Tiết Mục</a>
                <a href="#register" class="hover:text-indochineGold transition">Đăng Ký Vé</a>
            </nav>
            <div>
                <a href="#register" class="hidden sm:inline-block bg-indochineGold text-indochineDark font-semibold px-5 py-2 rounded-full shadow-lg hover:bg-yellow-500 transition duration-300">
                    Nhận Vé Ngay
                </a>
            </div>
        </div>
    </header>

    <section class="relative bg-indochineDark text-indochineCream py-24 px-4 sm:px-6 lg:px-8 overflow-hidden flex items-center justify-center min-h-[85vh]">
        <div class="absolute inset-0 opacity-15 bg-[radial-gradient(#D4AF37_1px,transparent_1px)] [background-size:16px_16px]"></div>
        <!-- Vòng hoa sen / hoa văn trang trí góc -->
        <div class="absolute top-4 left-4 opacity-20 text-indochineGold text-6xl pointer-events-none">
            <i class="fas fa-dharmachakra animate-spin" style="animation-duration: 30s;"></i>
        </div>
        <div class="absolute bottom-4 right-4 opacity-20 text-indochineGold text-6xl pointer-events-none">
            <i class="fas fa-dharmachakra animate-spin" style="animation-duration: 30s; animation-direction: reverse;"></i>
        </div>

        <div class="relative max-w-4xl mx-auto text-center z-10">
            <div class="inline-block px-4 py-1.5 mb-6 rounded-full border border-indochineGold/50 bg-indochineRed/30 text-indochineGold text-xs sm:text-sm uppercase tracking-widest font-semibold">
                Đêm hội nghệ thuật đỉnh cao
            </div>
            <h1 class="font-serif text-4xl sm:text-6xl lg:text-7xl font-extrabold mb-6 leading-tight">
                ÂM SẮC <span class="text-gold-gradient">QUÊ HƯƠNG</span>
            </h1>
            <p class="text-lg sm:text-xl text-gray-300 mb-10 max-w-2xl mx-auto font-light leading-relaxed">
                Nơi những giai điệu Trống đồng, Đàn tranh, Đàn bầu hòa quyện cùng nhịp đập hiện đại, đưa bạn trở về với hồn thiêng sông núi Việt.
            </p>

            <!-- Thẻ thông tin thời gian & địa điểm -->
            <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 bg-white/5 backdrop-blur-md p-6 rounded-2xl border border-indochineGold/30 mb-10 text-left">
                <div class="flex items-center space-x-4">
                    <div class="w-12 h-12 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold shrink-0">
                        <i class="far fa-calendar-alt text-xl"></i>
                    </div>
                    <div>
                        <div class="text-xs text-gray-400">Thời Gian</div>
                        <div class="font-semibold text-sm sm:text-base text-indochineCream">20:00 - 22:30, 20/11/2026</div>
                    </div>
                </div>
                <div class="flex items-center space-x-4">
                    <div class="w-12 h-12 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold shrink-0">
                        <i class="fas fa-map-marker-alt text-xl"></i>
                    </div>
                    <div>
                        <div class="text-xs text-gray-400">Địa Điểm</div>
                        <div class="font-semibold text-sm sm:text-base text-indochineCream">Nhà Hát Lớn Thành Phố</div>
                    </div>
                </div>
                <div class="flex items-center space-x-4">
                    <div class="w-12 h-12 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold shrink-0">
                        <i class="fas fa-ticket-alt text-xl"></i>
                    </div>
                    <div>
                        <div class="text-xs text-gray-400">Loại Vé</div>
                        <div class="font-semibold text-sm sm:text-base text-indochineGold">Miễn Phí Tham Dự</div>
                    </div>
                </div>
            </div>

            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#register" class="bg-indochineGold text-indochineDark font-bold px-8 py-4 rounded-full shadow-xl hover:bg-yellow-400 transition duration-300 text-base">
                    Đăng Ký Tham Dự Ngay
                </a>
                <a href="#program" class="border border-indochineGold/70 text-indochineCream font-semibold px-8 py-4 rounded-full hover:bg-white/10 transition duration-300 text-base">
                    Khám Phá Chương Trình
                </a>
            </div>
        </div>
    </section>

    <section id="host" class="py-20 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto">
        <div class="text-center mb-16">
            <span class="text-indochineRed font-bold tracking-widest text-xs uppercase block mb-2">Người Tổ Chức & Chủ Trì</span>
            <h2 class="font-serif text-3xl sm:text-4xl font-bold text-indochineDark">Chân Dung Nghệ Sĩ Trưởng Ban</h2>
            <div class="w-24 h-1 bg-indochineGold mx-auto mt-4 rounded-full"></div>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center bg-white rounded-3xl p-8 sm:p-12 shadow-xl border border-indochineGold/20">
            <!-- Khung Ảnh Bản Thân / Chủ Trì -->
            <div class="lg:col-span-5 flex justify-center">
                <div class="relative">
                    <div class="absolute -inset-3 bg-gradient-to-r from-indochineRed to-indochineGold rounded-2xl blur-sm opacity-50"></div>
                    <div class="relative w-64 h-80 sm:w-72 sm:h-96 rounded-2xl overflow-hidden border-4 border-white shadow-2xl bg-indochineDark">
                        <!-- Hình ảnh nghệ sĩ chủ trì (có thể thay thế ảnh) -->
                        <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?auto=format&fit=crop&q=80&w=800" 
                             alt="Chân dung nghệ sĩ chủ trì" 
                             onerror="this.src='https://placehold.co/400x500/800020/D4AF37?text=Nghệ+Sĩ+Chủ+Trì'"
                             class="w-full h-full object-cover">
                        <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-4 text-center">
                            <span class="text-indochineGold text-sm font-semibold tracking-wide">NS. Nguyễn Mai Hương</span>
                            <p class="text-xs text-gray-200">Chủ nhiệm dự án Hồn Việt</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Nội dung lời chào & tiểu sử -->
            <div class="lg:col-span-7 space-y-6">
                <div class="inline-block px-3 py-1 rounded bg-indochineRed/10 text-indochineRed text-sm font-medium">
                    <i class="fas fa-quote-left mr-2"></i>Lời Chào Từ Ban Tổ Chức
                </div>
                <h3 class="font-serif text-2xl sm:text-3xl font-bold text-indochineDark">
                    "Giữ gìn ngọn lửa văn hóa truyền thống qua từng nốt nhạc."
                </h3>
                <p class="text-gray-600 leading-relaxed text-sm sm:text-base">
                    Kính thưa quý vị yêu âm nhạc truyền thống, âm nhạc dân tộc không chỉ là tiếng lòng của ông cha ta qua ngàn đời, mà còn là bản sắc, là linh hồn của đất nước Việt Nam. Đêm hội này được tổ chức với mong muốn kết nối những trái tim đồng điệu, sống lại những khoảnh khắc tự hào bên tà áo dài, chiếc nón lá và âm hưởng mộc mạc mà thiêng liêng.
                </p>
                <p class="text-gray-600 leading-relaxed text-sm sm:text-base">
                    Sự hiện diện của quý vị là nguồn động lực lớn lao để chúng tôi tiếp tục hành trình lan tỏa giá trị văn hóa dân gian đến với đông đảo khán giả mọi thế hệ.
                </p>
                
                <div class="pt-4 flex items-center space-x-6 border-t border-gray-100">
                    <div>
                        <div class="font-serif font-bold text-indochineRed text-xl">15+</div>
                        <div class="text-xs text-gray-500">Năm gắn bó nghệ thuật</div>
                    </div>
                    <div class="h-8 w-px bg-gray-200"></div>
                    <div>
                        <div class="font-serif font-bold text-indochineRed text-xl">30+</div>
                        <div class="text-xs text-gray-500">Nghệ sĩ tham gia</div>
                    </div>
                    <div class="h-8 w-px bg-gray-200"></div>
                    <div>
                        <div class="font-serif font-bold text-indochineRed text-xl">1,000+</div>
                        <div class="text-xs text-gray-500">Khán giả đồng hành</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="program" class="py-20 bg-indochineDark text-indochineCream px-4 sm:px-6 lg:px-8 relative overflow-hidden">
        <div class="max-w-7xl mx-auto relative z-10">
            <div class="text-center mb-16">
                <span class="text-indochineGold font-bold tracking-widest text-xs uppercase block mb-2">Đặc Sắc Đêm Hội</span>
                <h2 class="font-serif text-3xl sm:text-4xl font-bold">Nhạc Cụ & Tiết Mục Chính</h2>
                <div class="w-24 h-1 bg-indochineGold mx-auto mt-4 rounded-full"></div>
            </div>

            <!-- Danh sách nhạc cụ nổi bật -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 mb-16">
                <!-- Nhạc cụ 1 -->
                <div class="bg-white/5 border border-indochineGold/30 rounded-2xl p-6 hover:bg-white/10 transition duration-300">
                    <div class="w-14 h-14 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold text-2xl mb-6">
                        <i class="fas fa-guitar"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold mb-2 text-indochineGold">Đàn Tranh</h3>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Tiếng đàn trong trẻo như tiếng suối ngàn, mang âm hưởng cung đình uy nghi kết hợp với nét trữ tình dân gian ba miền.
                    </p>
                </div>
                <!-- Nhạc cụ 2 -->
                <div class="bg-white/5 border border-indochineGold/30 rounded-2xl p-6 hover:bg-white/10 transition duration-300">
                    <div class="w-14 h-14 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold text-2xl mb-6">
                        <i class="fas fa-music"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold mb-2 text-indochineGold">Đàn Bầu</h3>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Chỉ với một dây và cần uốn nắn, đàn bầu chạm đến tận cùng cảm xúc người nghe bằng âm vực ngọt ngào, sâu lắng như lời ru của mẹ.
                    </p>
                </div>
                <!-- Nhạc cụ 3 -->
                <div class="bg-white/5 border border-indochineGold/30 rounded-2xl p-6 hover:bg-white/10 transition duration-300">
                    <div class="w-14 h-14 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold text-2xl mb-6">
                        <i class="fas fa-wind"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold mb-2 text-indochineGold">Sáo Trúc & Tiêu</h3>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Tiếng sáo vi vu gợi mở không gian làng quê thanh bình với cánh cò bay lả và những buổi chiều hè lộng gió miền quê Bắc Bộ.
                    </p>
                </div>
                <!-- Nhạc cụ 4 -->
                <div class="bg-white/5 border border-indochineGold/30 rounded-2xl p-6 hover:bg-white/10 transition duration-300">
                    <div class="w-14 h-14 rounded-xl bg-indochineRed flex items-center justify-center text-indochineGold text-2xl mb-6">
                        <i class="fas fa-drum"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold mb-2 text-indochineGold">Trống Đồng & Cồng Chiêng</h3>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Âm vang hùng tráng từ ngàn xưa, tái hiện hào khí Tây Nguyên đại ngàn và âm hưởng trống hội rộn rã sắc xuân.
                    </p>
                </div>
            </div>

            <!-- Lịch trình tiết mục tóm tắt -->
            <div class="bg-gradient-to-r from-indochineRed/40 to-indochineDark border border-indochineGold/40 rounded-3xl p-8 sm:p-12">
                <h3 class="font-serif text-2xl font-bold mb-6 text-center text-indochineGold">Chương Trình Đêm Hội</h3>
                <div class="space-y-4 max-w-3xl mx-auto">
                    <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center border-b border-white/10 pb-4">
                        <div>
                            <span class="text-indochineGold font-semibold">20:00 - 20:30</span>
                            <h4 class="font-bold text-lg">Khai hội: Trống hội âm vang & Múa sen chào mừng</h4>
                        </div>
                        <span class="text-xs bg-white/10 px-3 py-1 rounded-full text-gray-300 mt-2 sm:mt-0">Sân khấu chính</span>
                    </div>
                    <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center border-b border-white/10 pb-4">
                        <div>
                            <span class="text-indochineGold font-semibold">20:30 - 21:15</span>
                            <h4 class="font-bold text-lg">Hòa tấu nhạc cụ dân tộc & Độc tấu đàn bầu "Bèo dạt mây trôi"</h4>
                        </div>
                        <span class="text-xs bg-white/10 px-3 py-1 rounded-full text-gray-300 mt-2 sm:mt-0">Phần 1</span>
                    </div>
                    <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center border-b border-white/10 pb-4">
                        <div>
                            <span class="text-indochineGold font-semibold">21:15 - 22:00</span>
                            <h4 class="font-bold text-lg">Giao lưu nghệ sĩ & Trình diễn âm hưởng Tây Nguyên</h4>
                        </div>
                        <span class="text-xs bg-white/10 px-3 py-1 rounded-full text-gray-300 mt-2 sm:mt-0">Phần 2</span>
                    </div>
                    <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center">
                        <div>
                            <span class="text-indochineGold font-semibold">22:00 - 22:30</span>
                            <h4 class="font-bold text-lg">Hợp xưởng bế mạc "Lên ngàn" & Tri ân khán giả</h4>
                        </div>
                        <span class="text-xs bg-white/10 px-3 py-1 rounded-full text-gray-300 mt-2 sm:mt-0">Bế mạc</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="register" class="py-20 px-4 sm:px-6 lg:px-8 max-w-4xl mx-auto">
        <div class="text-center mb-16">
            <span class="text-indochineRed font-bold tracking-widest text-xs uppercase block mb-2">Giữ Chỗ Ngồi Sớm</span>
            <h2 class="font-serif text-3xl sm:text-4xl font-bold text-indochineDark">Đăng Ký Tham Dự Đêm Hội</h2>
            <div class="w-24 h-1 bg-indochineGold mx-auto mt-4 rounded-full"></div>
            <p class="text-gray-600 mt-4 max-w-lg mx-auto text-sm sm:text-base">
                Vui lòng điền thông tin bên dưới để Ban Tổ Chức gửi vé mời điện tử qua Email hoặc số điện thoại của bạn.
            </p>
        </div>

        <div class="bg-white rounded-3xl p-8 sm:p-12 shadow-2xl border border-indochineGold/30 relative">
            
            <!-- Form Đăng Ký -->
            <form id="registrationForm" class="space-y-6" onsubmit="handleFormSubmit(event)">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-sm font-medium text-indochineDark mb-2" for="fullname">Họ và Tên *</label>
                        <input type="text" id="fullname" required 
                               class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-indochineRed focus:ring-2 focus:ring-indochineRed/20 outline-none transition"
                               placeholder="Nguyễn Văn A">
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-indochineDark mb-2" for="phone">Số Điện Thoại *</label>
                        <input type="tel" id="phone" required 
                               class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-indochineRed focus:ring-2 focus:ring-indochineRed/20 outline-none transition"
                               placeholder="09123456xx">
                    </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                    <div>
                        <label class="block text-sm font-medium text-indochineDark mb-2" for="email">Địa Chỉ Email *</label>
                        <input type="email" id="email" required 
                               class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-indochineRed focus:ring-2 focus:ring-indochineRed/20 outline-none transition"
                               placeholder="example@email.com">
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-indochineDark mb-2" for="tickets">Số Lượng Ghế Ngồi *</label>
                        <select id="tickets" class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-indochineRed focus:ring-2 focus:ring-indochineRed/20 outline-none transition bg-white">
                            <option value="1">1 Vé (Ghế đơn)</option>
                            <option value="2">2 Vé (Cặp đôi)</option>
                            <option value="3">3 Vé (Nhóm nhỏ)</option>
                            <option value="4">4 Vé (Gia đình)</option>
                        </select>
                    </div>
                </div>

                <div>
                    <label class="block text-sm font-medium text-indochineDark mb-2" for="note">Lời nhắn hoặc yêu cầu đặc biệt (Không bắt buộc)</label>
                    <textarea id="note" rows="3" 
                              class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-indochineRed focus:ring-2 focus:ring-indochineRed/20 outline-none transition"
                              placeholder="Tôi rất mong đợi tiết mục đàn bầu..."></textarea>
                </div>

                <div class="text-center pt-4">
                    <button type="submit" class="w-full sm:w-auto bg-indochineRed text-indochineGold font-bold px-10 py-4 rounded-full shadow-xl hover:bg-red-900 transition duration-300 text-base">
                        Gửi Đăng Ký Nhận Vé
                    </button>
                </div>
            </form>

            <!-- Thông báo thành công (Ẩn mặc định) -->
            <div id="successMessage" class="hidden text-center py-12 space-y-4">
                <div class="w-20 h-20 bg-green-100 text-indochineGreen rounded-full flex items-center justify-center mx-auto text-3xl shadow-inner">
                    <i class="fas fa-check"></i>
                </div>
                <h3 class="font-serif text-3xl font-bold text-indochineDark">Đăng Ký Thành Công!</h3>
                <p class="text-gray-600 max-w-md mx-auto text-sm sm:text-base">
                    Cảm ơn bạn đã đăng ký tham dự <strong>Đêm Hội Nhạc Dân Tộc</strong>. Ban tổ chức đã ghi nhận thông tin và sẽ gửi vé mời điện tử qua email của bạn trong thời gian sớm nhất.
                </p>
                <div class="pt-4">
                    <button onclick="resetForm()" class="bg-indochineDark text-indochineGold px-6 py-2.5 rounded-full text-sm font-semibold hover:bg-black transition">
                        Đăng Ký Thêm Người
                    </button>
                </div>
            </div>

        </div>
    </section>

    <footer class="bg-indochineDark text-indochineCream pt-16 pb-12 border-t border-indochineGold/30 mt-auto">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-3 gap-12 mb-12">
            <div>
                <div class="flex items-center space-x-3 mb-4">
                    <div class="w-8 h-8 rounded-full border border-indochineGold flex items-center justify-center bg-indochineRed">
                        <i class="fas fa-music text-indochineGold text-xs"></i>
                    </div>
                    <span class="font-serif text-lg font-bold text-indochineGold">HỒN VIỆT</span>
                </div>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Đêm hội tôn vinh giá trị âm nhạc truyền thống Việt Nam, kết nối thế hệ trẻ với di sản văn hóa ông cha.
                </p>
            </div>
            <div>
                <h4 class="font-serif font-bold text-indochineGold text-base mb-4">Liên Hệ Ban Tổ Chức</h4>
                <ul class="space-y-3 text-sm text-gray-300">
                    <li class="flex items-center space-x-3">
                        <i class="fas fa-map-marker-alt text-indochineGold"></i>
                        <span>Nhà Hát Lớn Thành Phố, Quận 1, TP.HCM</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <i class="fas fa-phone-alt text-indochineGold"></i>
                        <span>Hotline: 0909 123 456 (NS. Mai Hương)</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <i class="fas fa-envelope text-indochineGold"></i>
                        <span>lienhe@honvietmusic.vn</span>
                    </li>
                </ul>
            </div>
            <div>
                <h4 class="font-serif font-bold text-indochineGold text-base mb-4">Mạng Xã Hội</h4>
                <p class="text-sm text-gray-300 mb-4">Theo dõi trang fanpage chính thức để cập nhật hình ảnh và video buổi diễn.</p>
                <div class="flex space-x-4">
                    <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-indochineGold hover:text-indochineDark transition"><i class="fab fa-facebook-f"></i></a>
                    <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-indochineGold hover:text-indochineDark transition"><i class="fab fa-youtube"></i></a>
                    <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-indochineGold hover:text-indochineDark transition"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-indochineGold hover:text-indochineDark transition"><i class="fab fa-tiktok"></i></a>
                </div>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-white/10 pt-6 text-center text-xs text-gray-400">
            &copy; 2026 Đêm Hội Nhạc Dân Tộc Hồn Việt. Bản quyền thuộc về Ban tổ chức.
        </div>
    </footer>

    <script>
        function handleFormSubmit(event) {
            event.preventDefault();
            
            // Ẩn form và hiển thị thông báo thành công với hiệu ứng mượt mà
            const form = document.getElementById('registrationForm');
            const successMsg = document.getElementById('successMessage');
            
            form.style.display = 'none';
            successMsg.classList.remove('hidden');
            
            // Cuộn mượt lên vị trí thông báo thành công
            successMsg.scrollIntoView({ behavior: 'smooth', block: 'center' });
        }

        function resetForm() {
            const form = document.getElementById('registrationForm');
            const successMsg = document.getElementById('successMessage');
            
            form.reset();
            form.style.display = 'block';
            successMsg.classList.add('hidden');
        }
    </script>
</body>
</html>
