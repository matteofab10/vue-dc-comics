<template>
  <footer>
    <div class="container footer-top">
      <div class="list">
        <div class="column-list">
          <h3>DC COMICS</h3>
          <ul class="footer-list">
            <li><a href="">Characters</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">Films</a></li>
            <li><a href="">News</a></li>
            <li><a href="">TV</a></li>
          </ul>

          <h3>SHOP</h3>
          <ul class="footer-list">
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="column-list">
          <h3>DC</h3>
          <ul class="footer-list">
            <li><a href="">Terms Of Use</a></li>
            <li><a href="">Privacy policy(New)</a></li>
            <li><a href="">Ad Choices</a></li>
            <li><a href="">Advertising</a></li>
            <li><a href="">Jobs</a></li>
            <li><a href="">Subscriptions</a></li>
            <li><a href="">Talent Workshops</a></li>
            <li><a href="">CPSC Certificates</a></li>
            <li><a href="">Ratings</a></li>
            <li><a href="">Shop Help</a></li>
            <li><a href="">Contact Us</a></li>
          </ul>
        </div>
        <div class="column-list">
          <h3>SITES</h3>
          <ul class="footer-list">
            <li><a href="">DC</a></li>
            <li><a href="">MAD Magazine</a></li>
            <li><a href="">DC Kids</a></li>
            <li><a href="">DC Universe</a></li>
            <li><a href="">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-img">
        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container">
        <button>SIGN-UP NOW!</button>
        <div class="footer-social">
          <h3>FOLLOW US</h3>
          <img src="../assets/img/footer-facebook.png" alt="facebook">
          <img src="../assets/img/footer-twitter.png" alt="twitter">
          <img src="../assets/img/footer-youtube.png" alt="youtube">
          <img src="../assets/img/footer-pinterest.png" alt="pinterest">
          <img src="../assets/img/footer-periscope.png" alt="periscope">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style lang="scss">
  @import "../assets/style/vars.scss";

    footer {
    background-image: url("../assets/img/footer-bg.jpg");

      .footer-top {
        justify-content: space-between;
        align-items: center;
        overflow: hidden;
        height: 400px;
        color: white;
        display: flex;
        .list {
          display: flex;
          .column-list {
            margin-right: 30px;
            .footer-list {
              list-style: none;
              display: flex;
              flex-direction: column;
              li {
                padding: 2px 0;
                a {
                  color: rgb(189, 189, 189);
                  text-decoration: none;
                  &:hover {
                    color: white;
                    border-bottom: none;
                  }
                }
              }
            }
          }
        }
        h3 {
          font-size: 25px;
          margin: 10px 0;
        }
      } 
  }
  .footer-img {
    img {
      width: 100%;
    }
  }
  .footer-bottom {
    height: 108px;
    background-color: #303030;
    display: flex;
    align-items: center;
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      button {
        background-color: #303030;
        border: 2px solid $primary-color;
        color: white;
        padding: 15px;
        cursor: pointer;
      }
      .footer-social {
        display: flex;
        justify-content: space-between;
        align-items: center;
        h3 {
          color: $primary-color;
          font-size: 25px;
          margin-right: 10px;
        }
        img {
          width: 35px;
          margin: 0 12px;
          cursor: pointer;
        }
      }
    }
  }
</style>