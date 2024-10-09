<template>
    <div class="blog-container">
        <header class="blog-header">
            <h1 class="blog-title">Công Nghệ Thông Tin</h1>
            <p class="blog-subtitle">
                Cập nhật xu hướng và tin tức công nghệ mới nhất
            </p>
        </header>

        <section class="blog-content">
            <!-- Bài blog 1 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/trend.jpg" alt="Xu hướng công nghệ 1" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">
                        Xu hướng công nghệ trong năm 2024
                    </h2>
                    <p class="post-date">Ngày đăng: 09/10/2024</p>
                    <p class="post-description">
                        Năm 2024 hứa hẹn sẽ là năm của các công nghệ đột phá như
                        trí tuệ nhân tạo (AI), chuỗi khối (blockchain) và máy
                        tính lượng tử.
                    </p>
                </div>
            </article>

            <!-- Bài blog 2 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/secu.jpg" alt="Bảo mật" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">
                        Bảo mật thông tin trong kỷ nguyên số
                    </h2>
                    <p class="post-date">Ngày đăng: 05/10/2024</p>
                    <p class="post-description">
                        Tìm hiểu về các phương pháp bảo mật thông tin mới nhất
                        để bảo vệ doanh nghiệp và cá nhân.
                    </p>
                </div>
            </article>

            <!-- Bài blog 3 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/AI.jpg" alt="AI" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">
                        Sự phát triển của AI trong lĩnh vực công nghệ
                    </h2>
                    <p class="post-date">Ngày đăng: 03/10/2024</p>
                    <p class="post-description">
                        AI đang thay đổi cách con người làm việc và giao tiếp,
                        từ chăm sóc sức khỏe đến tự động hóa.
                    </p>
                </div>
            </article>

            <!-- Bài blog 4 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/quantum.jpg" alt="máy tính" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">Máy tính lượng tử</h2>
                    <p class="post-date">Ngày đăng: 01/10/2024</p>
                    <p class="post-description">
                        Máy tính lượng tử hứa hẹn giải quyết các bài toán mà máy
                        tính truyền thống không thể thực hiện.
                    </p>
                </div>
            </article>

            <!-- Bài blog 5 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/block.jpg" alt="Blockchain" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">Blockchain và tiềm năng</h2>
                    <p class="post-date">Ngày đăng: 25/09/2024</p>
                    <p class="post-description">
                        Công nghệ blockchain đang tạo ra một cuộc cách mạng về
                        bảo mật và minh bạch trong giao dịch.
                    </p>
                </div>
            </article>

            <!-- Bài blog 6 -->
            <article class="blog-post">
                <div class="post-image">
                    <img src="/images/future.jpg" alt="Tương lai" />
                </div>
                <div class="post-content">
                    <h2 class="post-title">Tương lai của công nghệ</h2>
                    <p class="post-date">Ngày đăng: 20/09/2024</p>
                    <p class="post-description">
                        Cùng tìm hiểu về những công nghệ sẽ định hình tương lai
                        của con người trong thế kỷ 21.
                    </p>
                </div>
            </article>
        </section>
        <br />
    </div>
</template>

<style scoped>
@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: translateY(-20px); /* Di chuyển lên trên */
    }
    100% {
        opacity: 1;
        transform: translateY(0); /* Trở về vị trí ban đầu */
    }
}

:root {
    --main-color: #0d47a1; /* Màu xanh dương đậm */
    --secondary-color: #1565c0; /* Màu xanh nhạt hơn */
    --background-color: #f5f5f5;
    --text-color: #ffffff;

    --transition: all 0.3s ease-in-out;
}

.blog-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    background-color: var(--background-color);
    font-family: "Roboto", sans-serif;
}

.blog-header {
    padding: 40px 20px;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    margin-bottom: 40px;
    color: var(--text-color);
    border-radius: 10px;
    background-color: #264b96;
    -webkit-text-fill-color: #efebeb;
    animation: fadeIn 0.5s ease forwards;
}

.blog-title {
    font-size: 42px;
    margin-bottom: 10px;
    font-weight: bold;
}

.blog-subtitle {
    font-size: 20px;
    font-weight: 300;
    margin-top: 10px;
}

.blog-content {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 40px;
}

.blog-post {
    border-radius: var(--border-radius);
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
    overflow: hidden;
    transition: var(--transition);
    position: relative;
    border-radius: 10px;
    animation: fadeIn 2s ease forwards;
}

.blog-post:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
}

.post-image {
    width: 100%;
    height: auto;
    object-fit: cover;
    transition: var(--transition);
}

.post-image img {
    width: 100%;
    height: auto;
    object-fit: cover;
    aspect-ratio: 16/9;
    border-radius: var(--border-radius);
}

.blog-post:hover .post-image img {
    transform: scale(1.05);
}

.post-image-circle {
    position: absolute;
    top: 20px;
    left: 20px;
    width: 100px;
    height: 100px;
    border-radius: 50%;
    overflow: hidden;
    border: 4px solid var(--text-color);
}

.post-image-circle img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.post-content {
    padding: 20px;
    color: var(--text-color);
}

.post-title {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 10px;
}

.post-date {
    font-size: 14px;
    color: var(--secondary-color);
    margin-bottom: 15px;
}

.post-description {
    font-size: 16px;
    line-height: 1.6;
    color: #aeb0b8;
}

/* Responsive */
@media (min-width: 768px) {
    .blog-content {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (min-width: 992px) {
    .blog-content {
        grid-template-columns: repeat(3, 1fr);
    }
}
</style>
