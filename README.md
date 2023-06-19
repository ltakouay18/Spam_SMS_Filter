# Spam_SMS_Filter
Project: Building a Spam Filter with Naive Bayes Algorithm

We are building a Naive Bayes Algorithm, derived from probability's Bayes theorem to train a dataset of existing sms messages that were classified by humans as 'spam' or 'ham' (Non-Spam).
Below is an illustration of the existing dataset and what we want our final training dataset to look like.
![image](https://github.com/ltakouay18/Spam_SMS_Filter/assets/129616564/65e2ded7-091d-4be8-9c34-0a63d5dd1447)

With Naive Bayes Algorithm we can answer two probability questions:
1. Probability of a New Message being a Spam given its content (w_{1}, w~2,..., w~n).
2. Probability of a New Message being a ham (non-spam) given its content (w1, w2,..., wn).

wn is a word in the sms message.
   
<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mtable displaystyle="true">
    <mlabeledtr>
      <mtd>
        <mtext>(4)</mtext>
      </mtd>
      <mtd>
        <mi>P</mi>
        <mo stretchy="false">(</mo>
        <msub>
          <mi>w</mi>
          <mi>i</mi>
        </msub>
        <mo data-mjx-texclass="ORD" stretchy="false">|</mo>
        <mi>H</mi>
        <mi>a</mi>
        <mi>m</mi>
        <mo stretchy="false">)</mo>
        <mo>=</mo>
        <mfrac>
          <mrow>
            <msub>
              <mi>N</mi>
              <mrow data-mjx-texclass="ORD">
                <msub>
                  <mi>w</mi>
                  <mi>i</mi>
                </msub>
                <mo data-mjx-texclass="ORD" stretchy="false">|</mo>
                <mi>H</mi>
                <mi>a</mi>
                <mi>m</mi>
              </mrow>
            </msub>
            <mo>+</mo>
            <mi>&#x3B1;</mi>
          </mrow>
          <mrow>
            <msub>
              <mi>N</mi>
              <mrow data-mjx-texclass="ORD">
                <mi>H</mi>
                <mi>a</mi>
                <mi>m</mi>
              </mrow>
            </msub>
            <mo>+</mo>
            <mi>&#x3B1;</mi>
            <mo>&#x22C5;</mo>
            <msub>
              <mi>N</mi>
              <mrow data-mjx-texclass="ORD">
                <mi>V</mi>
                <mi>o</mi>
                <mi>c</mi>
                <mi>a</mi>
                <mi>b</mi>
                <mi>u</mi>
                <mi>l</mi>
                <mi>a</mi>
                <mi>r</mi>
                <mi>y</mi>
              </mrow>
            </msub>
          </mrow>
        </mfrac>
      </mtd>
    </mlabeledtr>
  </mtable>
</math>

