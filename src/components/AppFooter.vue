<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <main>
    <div class="container">
      <div class="col-links">
        <div class="col-small">
          <div class="section">
            <h2>DC COMICS</h2>
            <ul>
              <li><a href="http://">Characters</a></li>
              <li><a href="http://">Comics</a></li>
              <li><a href="http://">Movies</a></li>
              <li><a href="http://">Tv</a></li>
              <li><a href="http://">Games</a></li>
              <li><a href="http://">Videos</a></li>
              <li><a href="http://">News</a></li>
            </ul>
          </div>
          <div class="section">
            <h2>SHOP</h2>
            <ul>
              <li><a href="http://">Shop DC</a></li>
              <li><a href="http://">Shop DC Collectibles</a></li>
            </ul>
          </div>
        </div>
        <div class="col-small">
          <h2>DC</h2>
          <ul>
            <li><a href="http://">Terms Of Use</a></li>
            <li><a href="http://">Privacy policy (New)</a></li>
            <li><a href="http://">Ad Choices</a></li>
            <li><a href="http://">Advertising</a></li>
            <li><a href="http://">Jobs</a></li>
            <li><a href="http://">Subscriptions</a></li>
            <li><a href="http://">Talent Workshops</a></li>
            <li><a href="http://">CPSC Certificates</a></li>
            <li><a href="http://">Ratings</a></li>
            <li><a href="http://">Shop Help</a></li>
            <li><a href="http://">Contact Us</a></li>
          </ul>
        </div>
        <div class="col-small">
          <h2>SITES</h2>
          <ul>
            <li><a href="http://">DC</a></li>
            <li><a href="http://">MAD Magazine</a></li>
            <li><a href="http://">DC Kids</a></li>
            <li><a href="http://">DC Universe</a></li>
            <li><a href="http://">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <img src="../assets/img/dc-logo-bg.png" alt="" />
    </div>
  </main>
  <footer>
    <div class="container">
      <div class="sign-up">
        <button type="button">SIGN UP NOW!</button>
      </div>

      <div class="follow">
        <h4>FOLLOW US</h4>
        <ul>
          <li>
            <a href="http://"
              ><img src="../assets/img/footer-facebook.png" alt=""
            /></a>
          </li>
          <li>
            <a href="http://"
              ><img src="../assets/img/footer-twitter.png" alt=""
            /></a>
          </li>
          <li>
            <a href="http://"
              ><img src="../assets/img/footer-youtube.png" alt=""
            /></a>
          </li>
          <li>
            <a href="http://"
              ><img src="../assets/img/footer-pinterest.png" alt=""
            /></a>
          </li>
          <li>
            <a href="http://"
              ><img src="../assets/img/footer-periscope.png" alt=""
            /></a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
main {
  background-image: url("../assets/img/footer-bg.jpg");

  background-repeat: no-repeat;
  background-size: cover;

  .container {
    padding: 20px 0;
    position: relative;
    display: flex;
    overflow: hidden;
    .col-links {
      color: var(--secondary-color);
      display: flex;
      width: 40%;

      .col-small {
        margin: 0 6px;
        width: calc(100% / 3);

        .section {
          padding-bottom: 10px;
        }

        ul {
          padding: 14px 0;
          list-style: none;

          li {
            padding: 4px 0;

            a {
              font-weight: 200;
              text-decoration: none;
              color: inherit;
            }
          }
        }
      }
    }

    img {
      top: -60px;
      right: 0;
      position: absolute;
    }
  }
}
footer {
  background-color: var(--quaternary-color);
  padding: 30px 0;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .sign-up {
      button {
        cursor: pointer;
        font-size: 18px;
        font-weight: 600;
        background-color: transparent;
        padding: 10px;
        color: var(--secondary-color);
        border: none;
        border: 2px solid var(--primary-color);
      }
    }

    .follow {
      display: flex;
      align-items: center;

      h4 {
        color: var(--primary-color);
        font-weight: 700;
      }

      ul {
        display: flex;
        list-style: none;

        li {
          padding: 0px 8px;

          a {
            font-weight: 200;
            text-decoration: none;
            color: inherit;
          }
        }
      }
    }
  }
}
</style>
