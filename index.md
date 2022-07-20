<style type="text/css">
   .wrapper {position: relative;}
   #input {position: absolute;top: 0;left: 0;opacity: 0;z-index: -10;}
</style>
<div class="wrapper">
   <p id="text">https://webpage-cn.eu.org/group</p>
   <textarea id="input"></textarea>
   <button onclick="copyText()">copy</button>
</div>
<script type="text/javascript">
    function copyText() {
      var text = document.getElementById("text").innerText;
      var input = document.getElementById("input");
      input.value = text;
      input.select();
      document.execCommand("复制");
    }
  </script>
