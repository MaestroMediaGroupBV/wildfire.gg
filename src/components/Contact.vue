<template>
  <div>
    <div id="svg"></div>
    <div class="container">
      <h1 class="title">Contact us</h1>
      <h2 class="subTitle">HAVE SOMETHING TO INQUIRE ABOUT? LET US KNOW!</h2>
      <p
        class="text"
      >If you want to ask any questions related to our organization or any of our teams, please contact us by using the form below, We will be happy to assist you in a timely manner.</p>
      <div class="content">
        <form name="contact" action method="post">
          <label class="form-label" for="name"></label>
          <input class="form-field" name="name" placeholder="Name" id="name">
          <label class="form-label" for="email"></label>
          <input class="form-field" name="email" placeholder="Email" id="email">
          <label class="form-label" for="message"></label>
          <textarea class="form-field" name="message" placeholder="Message 😊" id="message"></textarea>
          <input class="form-button" type="submit" value="SEND">
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact"
};
</script>

<style lang="scss" scoped>
.container {
  padding-left: 200px;
  padding-right: 200px;
  padding-bottom: 210px;
  padding-top: 200px;
  max-width: 650px;
  text-align: left;
  z-index: 1;
}
.title {
  @include resultsHeading;
  text-align: left;
}
.subTitle {
  @include resultsSubHeading;
}
.text {
  @include resultText;
  color: black;
  padding-top: 20px;
  padding-bottom: 20px;
  font-size: 16px;
}
.content {
  text-align: left;
}
form {
}
input {
  margin-top: 20px;
  font-size: 20px;
  border-radius: 0;
  padding: 10px;
  border-style: solid;
  border-color: black;
  border-width: 1px;
  width: 700px;
}
textarea {
  margin-top: 20px;
  font-size: 20px;
  padding: 10px;
  border-style: solid;
  border-color: black;
  border-width: 1px;
  width: 700px;
  height: 100px;
}
.form-button {
  background-color: $orange-title;
  color: white;
  width: 200px;
  border-style: none;
}
#svg {
  background-image: url("../assets/fire.svg");
  background-repeat: no-repeat;
  margin-left: 125vh;
  margin-bottom: -1200px;
  height: 1500px;
  overflow: hidden;
  align-self: right;
}
</style>