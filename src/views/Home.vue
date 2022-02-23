<template>
  <div class="home">
    <TheHeader class="mb-4"></TheHeader>

    <section class="banniere col-12 hero">
      <img
        src="../assets/heropic.png"
        alt="developer web png"
        class="devWebP"
      />

      <div class="hero-text">
        <p v-if="eng">Hi, my name is Adrien</p>
        <p v-else>Adrienと申します。</p>
        <br />

        <h1 class="pt-4 text-center" v-if="eng">
          I am a Web developer
          <br />
          <span class="typed-text">{{ typeValue }}</span>
          <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span>
        </h1>
        <h1 class="pt-4 text-center" v-else>
          Webデベロッパー
          <br />
          <span class="typed-text">{{ typeValue }}</span>
          <span class="cursor" :class="{ typing: typeStatus }">&nbsp;</span>
        </h1>
      </div>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1440 320"
        class="svg"
      >
        <path
          fill="#fff"
          fill-opacity="1"
          d="M0,192L48,170.7C96,149,192,107,288,122.7C384,139,480,213,576,229.3C672,245,768,203,864,192C960,181,1056,203,1152,224C1248,245,1344,267,1392,277.3L1440,288L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
        ></path>
      </svg>
    </section>

    <div class="container" id="aboutMe">
      <h2 class="mt-5 pt-3 text-center" v-if="eng">About me ✍🏻</h2>
      <h2 class="mt-5 pt-3 text-center" v-else>私について ✍🏻</h2>
      <img
        src="../assets/profilePic.jpg"
        alt="id picture"
        class="id-pic"
        data-aos="zoom-in"
        data-aos-duration="1800"
      />
      <p class="aboutMePar" v-if="eng">
        Inspired by the creative aspect of Web Developing, I recently graduated
        from an online program with Openclassrooms. I am mainly focused on
        frontend but I also acquired some skills in backend developement with
        Node Js (Express). I am really motivated and eager to learn, and most of
        all I enjoy coding. I used to live in France, China (3 years) and
        Australia (2 years), I am now based in Fukuoka Japan since 2019,
        although I recently passed the JLPT N2, I am still learning japanese
        every day. I can also speak english, french and chinese.
      </p>
      <p v-else>
        Web開発の創造的な側面に魅力を感じキャリアチェンジを決意しました。オンラインでITを学ぶ事ができるフランス政府認定の教育プログラムである、Openclassroomsを受講し2021年12月に無事卒業する事ができました(準学士号レベル)。
        私の強みは学習意欲の高さで主にフロントエンドに焦点を当てていますが、Node
        Js（Express）を使用してバックエンド開発のスキルも習得しています。
        そして何よりもコーディングを楽しんでいます。
        以前はフランス、中国（3年）、オーストラリア（2年）に住んでいた経験があり、英語、フランス語、中国語が話せます。2019年から福岡に拠点を移しており、2021年2月にJLPT
        N2に合格しました。現在JLPT N1 取得に向けて勉強を続けています。
      </p>
      <div class="text-center mb-5 pb-3">
        <a
          :href="`${publicPath}Benete2022.pdf`"
          class="btn btn-secondary text-center"
          download="Benete2022.pdf"
          v-if="eng"
          ><i class="fas fa-download"></i> Download my resume in PDF</a
        >
        <a
          :href="`${publicPath}履歴書2022.pdf`"
          class="btn btn-secondary text-center"
          download="履歴書2022.pdf"
          v-else
          ><i class="fas fa-download"></i> PDF履歴書をダウンロード</a
        >
      </div>

      <h2 class="text-center pb-3" v-if="eng">My Skills 💪🏻</h2>
      <h2 class="text-center pb-3" v-else>スキル 💪🏻</h2>
      <div class="text-center">
        <img
          src="../assets/html.png"
          alt="logo html"
          class="logo htmlD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="2400"
        />
        <img
          src="../assets/css.png"
          alt="logo css"
          class="logo css cssD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="2000"
        />
        <img
          src="../assets/js.png"
          alt="logo javascript"
          class="logo js jsD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="1800"
        />
        <img
          src="../assets/logo.png"
          alt="logo vue"
          class="logo vue vueD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="1600"
        />
        <img
          src="../assets/sass.png"
          alt="logo sass"
          class="logo sassD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="1400"
        />
        <img
          src="../assets/bootstrap.png"
          alt="logo bootstrap"
          class="logo bootstrapD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="1200"
        />
        <img
          src="../assets/mysql.png"
          alt="logo mysql"
          class="logo mysql mysqlD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
        />
        <img
          src="../assets/mongo.png"
          alt="logo mongodb"
          class="logo mongo mongoD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="800"
        />
        <img
          src="../assets/node.png"
          alt="logo node"
          class="logo node nodeD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="600"
        />
        <img
          src="../assets/lr.png"
          alt="logo lr"
          class="logo lr lrD mt-4"
          data-aos="zoom-in-up"
          data-aos-duration="400"
        />
      </div>
    </div>
    <br />
    <h2 class="text-center pt-4 mb-5 mt-3" id="myWorks" v-if="eng">
      My works <span>🚀</span>
    </h2>
    <h2 class="text-center pt-4 mb-5 mt-3" id="myWorks" v-else>
      プロジェクト <span>🚀</span>
    </h2>
    <br />
    <div class="works">
      <div class="card mb-5">
        <img
          class="card-img-top reservia"
          src="..\assets\reservia.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">Reservia</h5>
          <p class="card-text" v-if="eng">
            Turn Mock-ups Into a Web Page with HTML & CSS, implementing a travel
            booking platform's website from scratch. The page is responsive
          </p>
          <p class="card-text" v-else>
            モックアップをHTMLとCSSを使用してWebページに変換し、旅行予約プラットフォームのWebサイトを最初から実装します。ページはレスポンシブルです
          </p>
          <div class="pb-3">
            <img
              src="../assets/html.png"
              alt="logo html"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/css.png"
              alt="logo css"
              class="logo css"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://adriben.github.io/AdrienBenete_2_27072021/"
              class="btn btn-primary"
              >Check the webpage</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_2_27072021"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a
              href="https://adriben.github.io/AdrienBenete_2_27072021/"
              class="btn btn-primary"
              >Webページに移動する</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_2_27072021"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>

          <img
            class="iphone"
            src="../assets/iphone.png"
            alt="iphone picture"
            id="reservia"
          />
        </div>
      </div>
      <div class="card mb-5">
        <img
          class="card-img-top ohmyfood"
          src="..\assets\ohmyfood.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title">Ohmyfood</h5>
          <p class="card-text" v-if="eng">
            Integrate a mobile website with animations in CSS. Implement the
            mobile version of this foodtech website with CSS animations.
          </p>
          <p class="card-text" v-else>
            モバイルWebサイトをCSSのアニメーションと統合します。
            このフードテックウェブサイトのモバイル版をCSSアニメーションで実装する
          </p>
          <div class="pb-3">
            <img
              src="../assets/html.png"
              alt="logo html"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/css.png"
              alt="logo css"
              class="logo css"
              data-aos="fade-right"
            />
            <img
              src="../assets/sass.png"
              alt="logo sass"
              class="logo"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://adriben.github.io/AdrienBenete_3_15082021/"
              class="btn btn-primary"
              >Check the webpage</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_3_15082021"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a
              href="https://adriben.github.io/AdrienBenete_3_15082021/"
              class="btn btn-primary"
              >Webページに移動する</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_3_15082021"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
          <img
            class="iphone"
            src="../assets/iphone.png"
            alt="iphone picture"
            id="ohmyfood"
          />
        </div>
      </div>
      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\lachouetteagence.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">
            Optimize an Existing Website (La Chouette agence)
          </h5>
          <h5 class="card-title" v-else>
            既存のWebサイトを最適化します (La Chouette agence)
          </h5>
          <p class="card-text" v-if="eng">
            Research and implement current best practices and standards in web
            development, including SEO, size and speed, and accessibility.
          </p>
          <p class="card-text" v-else>
            SEO、サイズと速度、アクセシビリティなど、Web開発における現在のベストプラクティスと標準を調査して実装します
          </p>
          <div class="pb-3">
            <img
              src="../assets/seo.png"
              alt="logo seo"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/analytics.png"
              alt="logo analytics"
              class="logo analytics"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://github.com/adriben/AdrienBenete_4_27082021"
              class="btn btn-primary"
              >Code after optimization</a
            >
            <a
              href="https://github.com/adriben/chouetteAgenceBEFORE"
              class="btn btn-secondary ml-3"
              >Code before optimization</a
            >
          </div>
          <div v-else>
            <a
              href="https://github.com/adriben/AdrienBenete_4_27082021"
              class="btn btn-primary"
              >最適化後</a
            >
            <a
              href="https://github.com/adriben/chouetteAgenceBEFORE"
              class="btn btn-secondary ml-3"
              >最適化前</a
            >
          </div>

          <img
            class="performance"
            src="../assets/performance.png"
            alt="iphone picture"
            id="performance"
          />
        </div>
      </div>
      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\orinocamera.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">
            Built an e-commerce Website with JavaScript
          </h5>
          <h5 class="card-title" v-else>
            JavaScriptを使用してeコマースWebサイトを構築する
          </h5>
          <p class="card-text" v-if="eng">
            Created the design and use an API to collect information about
            products and add a cart feature for purchases. Utilisation of fetch,
            localstorage, I did all the front end part. It allowed me to learn
            and improve myself in vanilla javascript (no framework)
          </p>
          <p class="card-text" v-else>
            デザインを作成し、APIを使用して製品に関する情報を収集、購入用のカート機能を追加します。
            フェッチ、ローカルストレージを利用して、すべてのフロントエンド部分を実行しました。バニラジャバスクリプト（フレームワークなし)を使い自分自身で確認改善することができます
          </p>
          <div class="pb-3">
            <img
              src="../assets/html.png"
              alt="logo html"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/css.png"
              alt="logo css"
              class="logo css"
              data-aos="fade-right"
            />
            <img
              src="../assets/sass.png"
              alt="logo sass"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/bootstrap.png"
              alt="logo bootstrap"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/js.png"
              alt="logo javascript"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/ux.png"
              alt="logo design"
              class="logo ux"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a href="https://youtu.be/VQOkRmA3UsE" class="btn btn-primary mr-3"
              >Check the video Demo</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_5_27092021/tree/main/frontend"
              class="btn btn-secondary"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a href="https://youtu.be/VQOkRmA3UsE" class="btn btn-primary"
              >Youtubeビデオに移動する</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_5_27092021/tree/main/frontend"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>

      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\hotsauce.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">
            Built a Secure API for a Review App
          </h5>
          <h5 class="card-title" v-else>レビューアプリのAPIを構築する</h5>
          <p class="card-text" v-if="eng">
            Built the back end for a new app, Hot Takes, where customers review
            specialty hot sauces. Use Node.js, Express, and MongoDB to build its
            NoSQL database. Secure customer data by applying the OWASP web
            security standards.
          </p>
          <p class="card-text" v-else>
            新しいアプリ、Hot
            Takesのバックエンドを構築。ここでは、顧客が特製ホットソースをレビューします。
            Node.js、Express、およびMongoDBを使用して、NoSQLデータベースを構築します。
            またOWASP Webセキュリティ標準を適用して顧客データを保護します。
          </p>
          <div class="pb-3">
            <img
              src="../assets/node.png"
              alt="logo node"
              class="logo node"
              data-aos="fade-right"
            />
            <img
              src="../assets/mongo.png"
              alt="logo mongo"
              class="logo mongo"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a href="https://youtu.be/wP7ak2om1L8" class="btn btn-primary"
              >Check the video Demo</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_6_26102021/tree/main/backend"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a href="https://youtu.be/wP7ak2om1L8" class="btn btn-primary"
              >Youtubeビデオに移動する</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_6_26102021/tree/main/backend"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>

      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\groupomania.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">
            Built a Full-Stack Corporate Social Network
          </h5>
          <h5 class="card-title" v-else>
            フルスタックのソーシャルネットワークを構築する
          </h5>
          <p class="card-text" v-if="eng">
            Analyze a client’s needs to define the scope and features of a new
            application. With the help of a front-end framework (Vue.js), built
            a full-stack solution, including a SQL database. The user is able to
            share a post, like and comment.
          </p>
          <p class="card-text" v-else>
            クライアントのニーズを分析して、新しいアプリケーションの範囲と機能を定義します。
            フロントエンドフレームワーク（Vue.js）を使用して、SQLデータベースを含むフルスタックソリューションを構築します。
            ユーザーは、投稿、いいね、コメントを共有できます。
          </p>
          <div class="pb-3">
            <img
              src="../assets/logo.png"
              alt="logo vue"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/vuex.png"
              alt="logo vue"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/mysql.png"
              alt="logo mysql"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/node.png"
              alt="logo node"
              class="logo node"
              data-aos="fade-right"
            />
            <img
              src="../assets/ux.png"
              alt="logo design designGroupo"
              class="logo ux"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a href="https://youtu.be/2UmIfHTFXOA" class="btn btn-primary"
              >Check the video Demo</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_7_19112021-"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a href="https://youtu.be/2UmIfHTFXOA" class="btn btn-primary"
              >Youtubeビデオに移動する</a
            >
            <a
              href="https://github.com/adriben/AdrienBenete_7_19112021-"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>

      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\movieApp.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">Built a Movie search engine</h5>
          <h5 class="card-title" v-else>映画検索エンジンを構築する</h5>
          <p class="card-text" v-if="eng">
            Built the frontend of a Movie search engine like IMDB with Nuxt.js.
            Api call with axios to gather and display the datas, possibility to
            search and get details about a movie.
          </p>
          <p class="card-text" v-else>
            Nuxt.jsを使用してIMDBのような映画検索エンジンのフロントエンドをします。
            Apiは、axiosを使用してデータを収集する。映画の詳細を検索するのができます。
          </p>
          <div class="pb-3">
            <img
              src="../assets/nuxt.png"
              alt="logo nuxt"
              class="logo nuxt"
              data-aos="fade-right"
            />
            <img
              src="../assets/logo.png"
              alt="logo vue"
              class="logo vue"
              data-aos="fade-right"
            />
            <img
              src="../assets/ux.png"
              alt="logo design designGroupo"
              class="logo ux"
              data-aos="fade-right"
            />
            <img
              src="../assets/heroku.png"
              alt="logo heroku"
              class="logo heroku"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://great-movie-app.herokuapp.com/"
              class="btn btn-primary"
              >Check the webpage</a
            >

            <a
              href="https://github.com/adriben/movie-app"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a
              href="https://great-movie-app.herokuapp.com/"
              class="btn btn-primary"
              >Webページに移動する</a
            >

            <a
              href="https://github.com/adriben/movie-app"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>
      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\cyclingFukuoka.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">
            Built an interactive site about cycling
          </h5>
          <h5 class="card-title" v-else>サイクリングに関するウェブページ</h5>
          <p class="card-text" v-if="eng">
            Creation of a interactive website for people passionated about
            cycling in Japan and Fukuoka. Api call to gather and get the weather
            and use of a database to store the maps.(In developement)
          </p>
          <p class="card-text" v-else>
            福岡のサイクリングに人々のためのインタラクティブなウェブサイトの作成。
            天気を収集して取得し、データベースを使用して地図を保存するためのApi呼び出し（開発中）
          </p>
          <div class="pb-3">
            <img
              src="../assets/logo.png"
              alt="logo vue"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/js.png"
              alt="logo js"
              class="logo js"
              data-aos="fade-right"
            />

            <img
              src="../assets/ux.png"
              alt="logo design designGroupo"
              class="logo ux"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://github.com/adriben/cycling-fukuoka"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a
              href="https://github.com/adriben/cycling-fukuoka"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>
      <div class="card mb-5">
        <img
          class="card-img-top"
          src="..\assets\fukubook.png"
          alt="Card image cap"
        />
        <div class="card-body">
          <h5 class="card-title" v-if="eng">Built a full-stack EC website</h5>
          <h5 class="card-title" v-else>
            フルスタックのeコマースWebサイトを構築する
          </h5>
          <p class="card-text" v-if="eng">
            Creation of a website for people who are looking to exchange give or
            sell books in Fukuoka. With the help of a front-end framework
            (Vue.js), built a full-stack solution, including a NoSQL database.
            (In developement)
          </p>
          <p class="card-text" v-else>
            福岡で外国の本を交換したり、交換したりする人のためのウェブサイトを作成。フロントエンドフレームワーク（Vue.js）を使用して、NoSQLデータベースを含むフルスタックソリューションを構築します。（開発中）
          </p>
          <div class="pb-3">
            <img
              src="../assets/logo.png"
              alt="logo vue"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/vuex.png"
              alt="logo vue"
              class="logo"
              data-aos="fade-right"
            />
            <img
              src="../assets/node.png"
              alt="logo node"
              class="logo node"
              data-aos="fade-right"
            />
            <img
              src="../assets/mongo.png"
              alt="logo mongo"
              class="logo mongo"
              data-aos="fade-right"
            />
            <img
              src="../assets/ux.png"
              alt="logo design designGroupo"
              class="logo ux"
              data-aos="fade-right"
            />
          </div>
          <div v-if="eng">
            <a
              href="https://github.com/adriben/fukubook"
              class="btn btn-secondary ml-3"
              >Check the code</a
            >
          </div>
          <div v-else>
            <a
              href="https://github.com/adriben/fukubook"
              class="btn btn-secondary ml-3"
              >コードに移動する</a
            >
          </div>
        </div>
      </div>
    </div>
    <div class="black pt-4 bg-dark">
      <div class="text-center" id="contact">
        <h2 v-if="eng">Contact ☎️</h2>
        <h2 v-else>連絡先 ☎️</h2>
        <Contact></Contact>
      </div>
      <div class="text-center mt-4">
        <h3 v-if="eng">Hobbies 🏖</h3>
        <h3 v-else>趣味 🏖</h3>
        <Hobbies class="container pb-5"></Hobbies>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import TheHeader from "@/components/TheHeader.vue";
import Hobbies from "@/components/Hobbies.vue";
import Contact from "@/components/Contact.vue";

import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "Home",
  components: {
    TheHeader: TheHeader,
    Hobbies: Hobbies,
    Contact: Contact,
  },
  data: () => {
    return {
      typeValue: "",
      typeStatus: false,
      typeArray: ["Front end", "Full stack", "Design"],
      typingSpeed: 200,
      erasingSpeed: 100,
      newTextDelay: 1500,
      typeArrayIndex: 0,
      charIndex: 0,
      publicPath: process.env.BASE_URL,
      eng: true,
    };
  },
  methods: {
    typeText() {
      if (this.charIndex < this.typeArray[this.typeArrayIndex].length) {
        if (!this.typeStatus) this.typeStatus = true;
        this.typeValue += this.typeArray[this.typeArrayIndex].charAt(
          this.charIndex
        );
        this.charIndex += 1;

        setTimeout(this.typeText, this.typingSpeed);
      } else {
        this.typeStatus = false;
        setTimeout(this.eraseText, this.newTextDelay);
      }
    },
    eraseText() {
      if (this.charIndex > 0) {
        if (!this.typeStatus) this.typeStatus = true;

        this.typeValue = this.typeArray[this.typeArrayIndex].substring(
          0,
          this.charIndex - 1
        );
        this.charIndex -= 1;
        setTimeout(this.eraseText, this.erasingSpeed);
      } else {
        this.typeStatus = false;
        this.typeArrayIndex += 1;
        if (this.typeArrayIndex >= this.typeArray.length)
          this.typeArrayIndex = 0;

        setTimeout(this.typeText, this.typingSpeed + 1000);
      }
    },
    changeLang() {
      this.eng = !this.eng;
    },
  },

  created() {
    setTimeout(this.typeText, this.newTextDelay + 200);
    AOS.init();
  },
};
</script>
<style lang="scss">
.loader {
  z-index: 5;
  width: 100%;
  height: 100%;
  background-color: rgba(11, 12, 12, 0.541);
  position: fixed;
}

.spin {
  position: absolute;
  top: 50%;
  left: 50%;
  margin: 0 auto;
}
.home {
  background-color: rgba(255, 255, 255, 0.685);
}

img {
  width: 100%;

  margin: auto;
  max-width: 1700px;
  object-fit: cover;
}

.hero {
  color: white;
  background-image: linear-gradient(
    rgb(9, 164, 179),
    rgba(26, 108, 202, 0.842)
  );
  background-position: top;
  background-repeat: no-repeat;
  background-size: cover;
  height: 600px;
  width: 100%;
  position: relative;
  @media screen and (max-width: 900px) {
    height: 650px;
  }
  @media screen and (max-width: 450px) {
    height: 600px;
  }

  .hero-text {
    position: absolute;
    align-items: center;
    top: 40%;
    left: 45%;
    @media screen and (max-width: 1100px) {
      top: 30%;
      left: 55%;
    }
    @media screen and (max-width: 900px) {
      top: 20%;
      left: 20%;
    }
    @media screen and (max-width: 620px) {
      top: 20%;
      left: 10%;
    }
    @media screen and (max-width: 400px) {
      top: 30%;
      left: 0%;
    }
    p {
      position: absolute;
      font-size: 200%;
      top: -20%;
      left: 10%;
      animation: slideDisplay 3s;
    }
    h1 {
      animation: slideDisplay 500ms;

      span.cursor {
        display: inline-block;
        margin-left: 3px;
        width: 4px;
        background-color: #fff;
        animation: cursorBlink 800ms infinite;
      }
      span.cursor.typing {
        animation: none;
      }
      span.typed-text {
        color: #e27d60;
      }
    }
  }
}
.devWebP {
  width: 27rem;
  position: absolute;
  top: 40%;
  left: 10%;
  z-index: 10;
  @media screen and (max-width: 900px) {
    width: 20rem;
    top: 50%;
    left: 20%;
  }

  @media screen and (max-width: 580px) {
    top: 50%;
    left: 20%;
  }
  @media screen and (max-width: 400px) {
    top: 60%;
    left: 10%;
    width: 15rem;
  }
  @media screen and (max-width: 300px) {
    top: 60%;
    left: 0%;
    width: 15rem;
  }
}
.svg {
  position: absolute;
  top: 40%;
  left: 0%;
  z-index: 6;
  @media screen and (max-width: 1640px) {
    top: 50%;
    left: 0%;
  }
  @media screen and (max-width: 1440px) {
    top: 60%;
    left: 0%;
  }
  @media screen and (max-width: 1100px) {
    top: 70%;
    left: 0%;
  }
  @media screen and (max-width: 900px) {
    top: 80%;
    left: 0%;
  }
  @media screen and (max-width: 650px) {
    top: 85%;
    left: 0%;
  }
  @media screen and (max-width: 470px) {
    top: 87%;
    left: 0%;
  }
  @media screen and (max-width: 365px) {
    top: 90%;
    left: 0%;
  }
}
.banner {
  height: 700px;
}
#aboutMe {
  position: relative;
  z-index: 12;

  @media screen and (max-width: 1400px) {
    padding-top: 4rem;
  }
}
.id-pic {
  width: 8rem;
  height: 8rem;
  object-fit: cover;
  border-radius: 150px;
  position: absolute;
  left: -120px;
  top: 50px;
  z-index: 11;
  @media screen and (max-width: 1400px) {
    left: 40%;
    margin: 0 auto;
    top: 0px;
  }
}
.aboutMePar {
  font-size: 120%;
  font-family: "Fuzzy Bubbles", cursive;
}
.logo {
  width: 80px;
  padding-right: 1rem;
  transition: 100ms;

  &:hover {
    transform: scale(1.3);
    transition: 300ms;
    cursor: pointer;
  }
}
.css {
  width: 60px;
}

.btn-secondary {
  background-color: #d85c3ae0;
}

.works {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  @media screen and (max-width: 1900px) {
    grid-template-columns: 1fr 1fr;
  }
  @media screen and (max-width: 1300px) {
    grid-template-columns: 1fr;
  }
}

.card {
  width: 35rem;
  position: relative;
  z-index: 1;
  border-radius: 20px;
  box-shadow: 3px 3px 7px rgba(63, 62, 62, 0.596);
  transition: 400ms;
  @media screen and (max-width: 600px) {
    width: 100%;
    a.btn-secondary {
      margin-top: 0.8rem;
    }
    @media screen and (max-width: 400px) {
      width: 100%;
      border-radius: 0px;
      box-shadow: none;
      a.btn-secondary {
        margin-top: 0.8rem;
      }
    }
  }

  &:hover {
    transform: scale(1.05);
    transition: 400ms;
    @media screen and (max-width: 600px) {
      transform: scale(1);
    }
  }

  .card-img-top {
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
    height: 29rem;
    object-fit: cover;
    border-bottom: 1px solid rgba(128, 128, 128, 0.308);
    @media screen and (max-width: 400px) {
      border-radius: 0px;
    }
  }
  .logo {
    width: 60px;
    padding-right: 1rem;
    transition: 100ms;
  }
  .css {
    width: 50px;
  }
  .ux {
    width: 80px;
  }
  .analytics {
    width: 7rem;
  }
  .mongo {
    width: 9rem;
    padding-left: 1rem;
  }
  .node {
    width: 6rem;
  }
  .nuxt {
    width: 9rem;
  }
  .heroku {
    width: 3.5rem;
  }
  .reservia {
    object-fit: cover;
    object-position: left top;
  }
  .ohmyfood {
    object-fit: cover;
    object-position: left top;
  }
  .iphone {
    height: 16rem;
    width: 7.6rem;
    position: absolute;
    top: 235px;
    right: 20px;
    background-size: 8rem;
    border-radius: 15px;
    box-shadow: 5px 3px 5px rgba(63, 62, 62, 0.596);
    z-index: 3;
  }
  .performance {
    height: 16rem;
    width: 25rem;
    position: absolute;
    top: 220px;
    right: -20px;
    background-size: 8rem;
    border: grey 1px solid;
    border-radius: 15px;
    box-shadow: 5px 3px 5px rgba(63, 62, 62, 0.596);
    z-index: 3;
    @media screen and (max-width: 630px) {
      height: 10rem;
      width: 20rem;
      right: 20px;
      top: 320px;
    }
  }
  #reservia {
    background-image: url("../assets/reserviaIphone1.png");
  }
  #ohmyfood {
    background-image: url("../assets/Menu.png");
    background-repeat: no-repeat;
  }
}

.phone {
  animation: shake 3s;
  color: red;

  animation-iteration-count: infinite;
}
.black {
  color: rgb(255, 255, 255);

  @media screen and (min-width: 1100px) {
    border-radius: 40% 40% 0 0;
  }
}
@keyframes cursorBlink {
  49% {
    background-color: #fff;
  }
  50% {
    background-color: transparent;
  }
  99% {
    background-color: transparent;
  }
}
@keyframes slideDisplay {
  0% {
    transform: translateX(-100px);
    opacity: 0;
  }
  50% {
    transform: translateX(-100px);
    opacity: 0;
  }
  100% {
    transform: translateX(0);
    opacity: 1;
  }
}
</style>
