---
layout: post
title: 연락
permalink: /contact/
---
<style>
.contact-li {
    list-style: none;
}

.contact-input {
    width: 100%;
}

.contact-input:focus {
    outline:none;
    border-bottom: 1px solid #37c376;
}

.contact-label {
    display: block;
}

ul.contact-ul {
    margin: 0;
    padding: 10px;
}

 #submit {

    background-color: #37c376;
    opacity: 0.8;
    color: #eee;
    border: none;

}

#submit:hover {
    opacity: 1;
    cursor: pointer;
} 


#contact-form {
    border: 1px solid #aaa;
    margin-bottom: 1em;
}

</style>

문의사항이나 건의사항이 있으면 얼마든지 연락하십시오.

어떠한 내용도 괜찮습니다. 편하게 연락해 주세요.

<form id="contact-form" class="form" action="https://formspree.io/{{site.email}}" method="POST" enctype="multipart/form-data">
        <ul class="contact-ul">
            <li class="contact-li">
                <label class="contact-label" for="name">이름:</label>
                <input type="text" placeholder="이름을 적어주세요" id="name" class="contact-input" name="name" tabindex="1"/>
            </li>
            <li class="contact-li">
                <label class="contact-label" for="email">이메일:</label>
                <input type="email" placeholder="이메일을 적어주세요" id="email" class="contact-input" name="email" tabindex="2"/>
            </li>
            <li class="contact-li">
                <label class="contact-label" for="message">내용:</label>
                <textarea class="contact-textarea" placeholder="건의 또는 문의할 내용을 적어주세요" class="contact-input" rows="4" id="message" name="message" tabindex="3"></textarea>
            </li>
            <input class="button" type="submit" value="Send" id="submit"/>
        </ul>
        
        <input type="hidden" name='redirect_to' value="http://blog.webjeda.com/thank-you/" />
        
</form>

감사합니다.
