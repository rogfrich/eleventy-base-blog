---
layout: layouts/post.njk
title: Tip Calculator
templateClass: tmpl-post
eleventyNavigation:
  key: Tips
  order: Latest
---
<!-- <form>
<input id="test">
</form>
<button onclick=test()>Click me</button>
<script>
    function test() {
        var inputText = document.getElementById("test").value;
        alert(inputText);
        };
</script> -->


<div class="form-group mt-3">
    <label class="form-label" for="billTotal">Bill total</label>
    <input type="number" class="form-control" id="billTotal" required>
</div>
<div class="form-group mt-3">
    <label class="form-label">Tip percentage</label>
    <input type="number" class="form-control" id="tipPercentage" required>
</div>
<button class="btn btn-primary mt-3" onclick=calculateTip()>Calculate Tip</button>

<p class="mt-3" id="resultText"></p>

<script>
    function calculateTip() {
        var billTotal = parseFloat(
            document.getElementById("billTotal").value);
        var tipPercentage = parseFloat(
            document.getElementById("tipPercentage").value);

        var tip = (billTotal / 100) * tipPercentage;
        var billTotalIncludingTip = billTotal + tip;

        var resultText = `On a bill of <strong>£${billTotal.toFixed(2)}</strong> a tip of <strong>${tipPercentage}%</strong> is <strong>£${tip.toFixed(2)}</strong>, which brings the total bill to <strong>£${billTotalIncludingTip.toFixed(2)}</strong>`;

        document.getElementById("resultText").innerHTML = resultText;
    }

</script>