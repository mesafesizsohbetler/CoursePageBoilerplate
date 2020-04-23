---
layout: default
---

Here you can find sample main page.

{{site.description}}

{% if site.course_activated %}

<div id="passw">
        <div>
            <input type="password" id="password" onkeydown="if (event.keyCode == 13) document.getElementById('button').click()" />
            <!-- IMPORTANT! this part is so if you click enter, it works. -->
        </div>
        <div>
            <br/>
            <input id="button" type="button" value="Login" onclick="checkPassword()" />
        </div>
    </div>
<div id="HIDDENDIV" style="display: none;">t l
        
<iframe  name="jitsiConferenceFrame0" id="jitsiConferenceFrame0" allowfullscreen="true" style="min-height: 500px; width: 100%; border: 0px;" allow="camera; microphone" src="{{site.meeting_link}}"></iframe>
  </div>

{% endif %}


Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page).

<script src="js/md5.js"></script>
<script>
    function checkPassword() {
        if (md5(document.getElementById('password').value) == '6d52d8398f90baafacd72fca28c340bb') {
            document.getElementById('HIDDENDIV').style.display = 'block';
            document.getElementById('passw').style.display = 'none';
        } else {
            alert('Invalid Password!');
            password.setSelectionRange(0, password.value.length);
        }
    }
</script>
