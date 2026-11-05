* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: "Microsoft JhengHei", sans-serif;
    background-color: #f7f5f0;
    color: #333;
}

/* 頂部導覽列 */
.navbar {
    background-color: #5c4033;
    color: #fff;
    padding: 1rem 2rem;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
    margin-left: 1.5rem;
}

/* 主體 Grid 雙欄排版 (側邊欄 + 內容區) */
.layout-grid {
    display: grid;
    grid-template-columns: 280px 1fr;
    gap: 2rem;
    max-width: 1200px;
    margin: 2rem auto;
    padding: 0 1rem;
    min-height: 70vh;
}

/* 側邊欄樣式 */
.sidebar {
    background: #fff;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    height: fit-content;
}

/* 主內容區 */
.content-area {
    background: #fff;
    padding: 2.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}

.tab-pane {
    display: none;
}

.tab-pane.active {
    display: block;
}

/* RWD 響應式斷點：手機版自動改為單欄 */
@media (max-width: 768px) {
    .layout-grid {
        grid-template-columns: 1fr;
    }
}
/* 色彩、字型與元件裝飾 */
h1, h2, h3 {
    color: #5c4033;
    margin-bottom: 1rem;
}

p {
    line-height: 1.7;
    margin-bottom: 1rem;
}

.tab-menu {
    list-style: none;
    margin-top: 1rem;
}

.tab-menu li {
    margin-bottom: 0.8rem;
}

.tab-btn {
    display: block;
    padding: 10px 15px;
    color: #5c4033;
    text-decoration: none;
    border-radius: 6px;
    transition: background 0.2s;
}

.tab-btn:hover, .tab-btn.active {
    background-color: #5c4033;
    color: #fff;
}

.card {
    background: #f2ebe1;
    padding: 1rem;
    border-radius: 6px;
    margin-top: 1.5rem;
}

table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 1.5rem;
}

th, td {
    border: 1px solid #ddd;
    padding: 12px;
    text-align: left;
}

th {
    background-color: #f2ebe1;
    color: #5c4033;
}

.media-aspect-ratio {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
    height: 0;
    margin-top: 1rem;
}

.media-aspect-ratio iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 6px;
}

.pagination {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 3rem;
    padding-top: 1rem;
    border-top: 1px solid #eee;
}

.page-btn {
    padding: 8px 16px;
    background-color: #5c4033;
    color: #fff;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.page-btn:hover {
    background-color: #3e2a21;
}

.footer {
    text-align: center;
    padding: 1.5rem;
    background-color: #5c4033;
    color: #fff;
    margin-top: 3rem;
}

</body>
</html>
