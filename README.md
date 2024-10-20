# Market-simulator
This web is developed for calculating how many resources should prepare to product.

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>下拉框示例</title>
</head>
<body>

<h2>请选择一个选项：</h2>

<select id="mySelect" onchange="showSelectedValue()">
    <option value="">--请选择--</option>
    <option value="option1">选项一</option>
    <option value="option2">选项二</option>
    <option value="option3">选项三</option>
</select>

<p id="result"></p>

<script>
function showSelectedValue() {
    var select = document.getElementById("mySelect");
    var value = select.value;
    var text = select.options[select.selectedIndex].text;
    if (value) {
        document.getElementById("result").innerHTML = "你选择了：" + text + "（值：" + value + "）";
    } else {
        document.getElementById("result").innerHTML = "";
    }
}
</script>

</body>
</html>