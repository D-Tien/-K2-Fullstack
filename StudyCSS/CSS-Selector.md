# CSS SELECTOR – NOTE TỔNG HỢP

==================================================

## I. SELECTOR CƠ BẢN

/_ Selector cùng cấp (trong 1 thẻ HTML) _/
h1.title {
}

==================================================

## II. SELECTOR THEO VỊ TRÍ

/_ Selector nằm sau (General Sibling) _/
ul ~ p {
}

/_ Selector liền kề (Adjacent Sibling) _/
p + h2 {
}

==================================================

## III. ATTRIBUTE SELECTOR

/_ Có thuộc tính _/
a[target] {
}

/_ Giá trị chính xác _/
a[href="value"] {
}

/_ Bắt đầu bằng value _/
a[href^="value"] {
}

/_ Chứa value _/
a[href*="value"] {
}

/_ Kết thúc bằng value _/
a[href$="value"] {
}

==================================================

## IV. CHỌN PHẦN TỬ TRONG CLASS

/_ Chọn tất cả thẻ con bên trong .box _/
.box \* {
}

/_ Chỉ chọn thẻ .box _/
.box {
}

==================================================

## V. PSEUDO ELEMENT (PHẦN TỬ GIẢ)

/_ Cú pháp _/
selector::pseudo-element {
}

/_ Các pseudo-element _/
::before
::after
::first-letter
::first-line
::selection
::placeholder

/_ Ví dụ _/
.title::before {
content: attr(data-index);
}

==================================================

## VI. PSEUDO CLASS (TRẠNG THÁI GIẢ)

/_ Cú pháp _/
selector:pseudo-class {
}

/_ Tương tác _/
:hover
:active
:focus

/_ Loại trừ _/
:not(.class)

/_ Trạng thái form _/
:disabled
:focus

/_ Vị trí phần tử _/
:first-child
:last-child
:first-of-type
:last-of-type
:nth-child(n)

/_ Ví dụ _/
li:nth-child(2) {
}

==================================================

## VII. LƯU Ý QUAN TRỌNG

- :hover, :active → dùng cho tất cả thẻ HTML
- :focus → chỉ áp dụng cho form (input, textarea, button)
- Thẻ không phải form muốn dùng :focus → thêm:

tabindex="0"

==================================================

END
