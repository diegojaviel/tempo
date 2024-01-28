<script setup></script>

<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-section">
        <h3>Tempo Cafe</h3>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry. Lorem Ipsum has been the industry's standard dummy text ever
          since the 1500s, when an unknown printer took a galley of type and
          scrambled it to make a type specimen book.
        </p>
        <div class="social-icons">
          <img src="../assets/img/socials-link.png" alt="Socials" />
        </div>
      </div>
      <div class="footer-section">
        <h4>About</h4>
        <ul>
          <li>Menu</li>
          <li>Features</li>
          <li>News & Blogs</li>
          <li>Help & Support</li>
        </ul>
      </div>
      <div class="footer-section">
        <h4>Company</h4>
        <ul>
          <li>How we work</li>
          <li>Terms of service</li>
          <li>Pricing</li>
          <li>FAQ</li>
        </ul>
      </div>
      <div class="footer-section">
        <h4>Contact Us</h4>
        <p>
          Akshaya Nagar 1st Block 1st Cross,<br />
          Rammurthy Nagar, Bangalore-560016<br />
          +1 202-918-2132<br />
          hello@email.com<br />
          www.tempocafe.com
        </p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  background-image: url("../assets/img/fotter-img.png");
  background-repeat: no-repeat;
  background-size: cover;
}

footer::before {
  content: "";
  background: #442808;
  opacity: 0.9;
  width: 100%;
  height: 44.5rem;
  position: absolute;
}

.footer-content {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 7rem;
  padding: 10rem;
  color: #ffffff;
  position: relative;
  z-index: 1;
}

.footer-section h3 {
  font-family: var(--font-primary);
  font-size: 5.4rem;
  font-weight: 400;
  margin-bottom: 2rem;
}

.social-icons {
  margin-top: 2rem;
  cursor: pointer;
}
.footer-section h4 {
  font-size: 2.6rem;
  font-weight: 700;
  margin-bottom: 3rem;
}
.footer-section p {
  width: 38rem;
}

.footer-section ul li {
  margin-bottom: 1rem;
  width: 13.5rem;
  cursor: pointer;
  transition: 0.3s;
}

.footer-section ul li:hover {
  color: #f9c06a;
}
</style>
