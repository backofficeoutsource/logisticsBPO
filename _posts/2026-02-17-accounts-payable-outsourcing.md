html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: 'Inter', sans-serif;
  background: #f4f7fb;
  color: #1e293b;
  line-height: 1.7;
}

/* CONTAINER */
.section {
  padding: 90px 20px;
}

.container {
  max-width: 1100px;
  margin: auto;
}

/* BANNER */
.banner {
  position: relative;
  height: 85vh;
  background: url('https://images.unsplash.com/photo-1554224155-8d04cb21cd6c') center/cover no-repeat;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
}

.banner::before {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, rgba(0,0,0,0.75), rgba(0,0,0,0.55));
}

.banner-content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

.banner h1 {
  font-size: 52px;
  margin-bottom: 20px;
  font-weight: 700;
}

.banner p {
  font-size: 18px;
  opacity: 0.9;
}

.cta-btn {
  display: inline-block;
  margin-top: 25px;
  padding: 14px 32px;
  background: #2563eb;
  color: #fff;
  border-radius: 50px;
  text-decorati
