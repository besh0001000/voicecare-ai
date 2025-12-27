<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>VoiceCare AI</title>
</head>
<body style="font-family:Arial;text-align:center;padding:40px">

  <h1>🎙️ VoiceCare AI</h1>
  <p>مساعد صوتي ذكي يجاوبك بصوت واضح وبسيط</p>

  <!-- زر التحدث -->
  <button onclick="askGemini()"
    style="font-size:24px; padding:20px 40px; cursor:pointer; background-color:#4CAF50; color:white; border:none; border-radius:8px;">
    تحدث 🎤
  </button>

  <p style="margin-top:40px; color:gray;">
    Powered by Google Cloud & ElevenLabs
  </p>

  <script>
    // محاكاة استدعاء Gemini
    function askGemini() {
      // نص المستخدم (يمكن لاحقًا ربطه بميكروفون)
      let userText = "مرحبا، كيف يمكنني استخدام الخدمات الرقمية؟";

      // محاكاة إجابة Google Cloud Gemini
      let geminiResponse = "مرحبًا! يمكنك استخدام الخدمات الرقمية بكل سهولة عبر VoiceCare AI.";

      // نطق الإجابة بالعربي
      let msg = new SpeechSynthesisUtterance();
      msg.text = geminiResponse;
      msg.lang = 'ar-SA';
      msg.rate = 1;
      msg.pitch = 1;
      window.speechSynthesis.speak(msg);
    }
  </script>

</body>
</html>
