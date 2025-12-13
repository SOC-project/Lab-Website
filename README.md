# Lab-Website

## 開發者指南

本指南說明如何將新的專案添加到網站的首頁 (Home Page) 與服務頁面 (Service Page)。
🙂🙃🙂🙃🙂🙃以下內容皆為AI生成，如有錯誤請自行判斷🙂🙃🙂🙃🙂🙃

### 1. 如何將專案新增至首頁 (Home Page) 的 "OUR SERVICES"

**檔案位置:** `home_page.html`

請找到 `<section class="service-area">` 區塊內的 `<div class="service-box">` -> `<div class="row">`。
在 `row` 內新增一個 `col-lg-6 col-sm-6` 的區塊。
可以參照SOC組的方式建立。

**程式碼範例:**

```html
<div class="col-lg-6 col-sm-6">
    <!-- 將 href 替換為您的專案連結 -->
    <a href="YOUR_PROJECT_PAGE.html">
        <div class="single-service-box border-right mt-5 wow fadeInRight" data-wow-duration="1s" data-wow-delay="0.2s">
            <div class="service-img" style="height: 450px;">
                <!-- 建議圖片設定 style="height: 100%; object-fit: cover;" 以保持版面整齊 -->
                <img src="assets/img/YOUR_IMAGE.png" alt="img" style="height: 100%; object-fit: cover;">
            </div>
            <div class="service-text d-flex align-items-center">
                <!-- 設定您的圖示與標題 -->
                <img src="assets/img/YOUR_ICON.svg" alt="icon">
                <h3>YOUR PROJECT TITLE</h3>
            </div>
            <span></span>
        </div>
    </a>
</div>
```

### 2. 如何將專案新增至服務頁面 (Service Page)

**檔案位置:** `service.html`

請找到 `<div class="project-box">` 區塊 (通常位於 `<div class="tab-pane fade show active" id="home">` 內)。
直接在 `project-box` 內新增一個 `<a>` 標籤區塊。

**程式碼範例:**

```html
<!-- 將 href 替換為您的專案連結 -->
<a href="YOUR_PROJECT_PAGE.html" class="single-project-box">
    <div class="single-project-img" style="height: 450px;">
        <!-- 建議圖片高度設定為 450px -->
        <img src="assets/img/YOUR_IMAGE.png" alt="img">
    </div>
    <div class="project-category">
        <ul>
            <li><img src="assets/img/service-1.svg" alt="img"></li>
            <li>
                <p>YOUR TEAM NAME / CATEGORY</p>
            </li>
        </ul>
    </div>
    <div class="project-info">
        <h3>YOUR PROJECT TITLE</h3>
        <p>Short Description</p>
    </div>
</a>
```

### 注意事項

- 目前專案中的子項目產品頁面尚未建構完成，請開發者在連結時留意，或暫時連結至 `service-details.html` 作為範例。

