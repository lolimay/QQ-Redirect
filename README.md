# QQ-Redirect
a demo for calling QQ chat dialog (support both desktop and mobile situation)

# kernel code
````js
/// configrations
const qqid = '1404363070' // Change it to your own QQ Id

// main
const windows = 'tencent://message/?uin=' + qqid
const mobile = 'mqqwpa://im/chat?chat_type=wpa&uin=' + qqid + '&version=1&src_type=web&web_src=oicqzone.com'
if(device.desktop()) {
  window.location.href=windows
} else {
  window.location.href=mobile
}   
````
