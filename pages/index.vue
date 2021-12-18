<template>
  <div class="root" v-on:keyup.left="alert('')">
    <div class="one" v-if="show == 1">
      <div class="one_content">
        <img src="../static/img.png" />
        <p>Masuda Takumi</p>
        <h1>増田 拓海</h1>
      </div>
    </div>
    <div class="one" v-if="show == 2">
      <div class="one_content">
        <h1 style="margin-bottom: 20px">Skills</h1>
        <h2 style="margin-bottom: 5px">言語</h2>
        <div style="text-align: left">
          <p>HTML/CSS：それなりに</p>
          <p>JavaScript：最低限</p>
          <p>Python：自信あり</p>
          <p>Go：ちょっとかじった</p>
        </div>

        <h2 style="margin-top: 15px; margin-bottom: 5px">フレームワーク</h2>
        <div style="text-align: left">
          <p>Nuxt.js：一番得意かも</p>
          <p>Flask：実務経験あり</p>
          <p>Express：最低限</p>
          <p>Django：今書けるか微妙</p>
        </div>
        <h2 style="margin-top: 15px; margin-bottom: 5px">その他</h2>
        <div style="text-align: left">
          <p>簿記：日商簿記3級</p>
          <p>freee：個人事業主の確定申告経験</p>
        </div>
      </div>
    </div>
    <div class="one" v-if="show == 3">
      <div class="one_content">
        <h1 style="margin-bottom: 20px">Works</h1>
        <h2 style="margin-bottom: 5px">
          <a href="https://fukushiki-kakeibo.com">複式家計簿</a>
        </h2>

        <p>複式簿記で家計簿をつけることができるWebアプリです。</p>
        <p>Nuxt.js+Firebaseで開発しています。</p>
        <p>
          U22プログラミングコンテスト2021でスポンサー賞「PCAクラウド賞」を頂きました。
        </p>
        <h2 style="margin-top: 15px; margin-bottom: 5px">TownWith(閉鎖)</h2>
        <p>地域の魅力を伝えることができるWebサービスです。</p>
        <p>Flaskで開発しました。</p>
        <h2 style="margin-top: 15px; margin-bottom: 5px">ThinkShare(閉鎖)</h2>
        <p>プログラミングを始めて1本目にリリースしたSNSです。</p>
        <p>Pythonでフレームワークを使わずに開発しました。</p>
      </div>
    </div>
    <div class="one" v-if="show == 4">
      <div class="one_content">
        <h1 style="margin-bottom: 20px">History</h1>
        <div style="text-align: left">
          <p>2021/12~：？？？</p>
          <p>2021/11：U22プロコン スポンサー賞受賞</p>
          <p>2021/06・07：家計簿アプリの開発・公開</p>
          <p>2020/06：Flask+Vueの仕事を開始</p>
          <p>2020/04：N高入学</p>
          <p>2020/04：個人事業の開業届を提出</p>
        </div>
      </div>
    </div>
    <div class="one" v-if="show == 5">
      <div class="one_content">
        <h1 style="margin-bottom: 20px">Links</h1>
        <div style="text-align: left">
          <a href="https://twitter.com/takumi_mas"><p>Twitter</p></a>
          <a href="https://github.com/takumimas"><p>Github</p></a>
          <a href="https://www.wantedly.com/id/takumimas"><p>Wantedly</p></a>
          <a href="https://masublog.net/"><p>個人ブログ</p></a>
        </div>
      </div>
    </div>
    <div class="f">
      <div>
        <p v-if="show != 1" @click="show -= 1">戻る</p>
      </div>
      <div style="text-align: right">
        <p @click="show += 1" v-if="show != 5">進む</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.root {
  min-height: 100vh;
  width: 100vw;
  background-color: #48c774;
}
.f {
  height: 5vh;
  display: flex;
}
.f div {
  color: white;
  font-size: 1.1rem;
  width: 50vw;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 10px;
}
a {
  color: #FF3860;
}
.one {
  color: white;
  height: 95vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.one_content {
  text-align: center;
}
.one_content img {
  width: 140px;
  margin-bottom: 20px;
}
.one_content p {
  font-size: 1.2rem;
}
h1 {
  font-size: 2rem;
  font-weight: 500;
}
h2 {
  font-size: 1.4rem;
  font-weight: 400;
}
</style>

<script>
export default {
  data: function () {
    return {
      show: 1,
    };
  },
  mounted() {},
  methods: {},
};
</script>
