---
layout: home
title: STYLE MODELING FOR MULTI-SPEAKER ARTICULATION-TO-SPEECH
---

Submitted to ICASSP 2023 

<h3>Authors
</h3>

Miseul Kim, Zhenyu Piao, Jihyun Lee, Hong-goo Kang

<br />

<h3>Proposed Method</h3>
<img src="./assets/img/Proposed_v5.png">

In this paper, we propose a neural articulation-to-speech
(ATS) framework that synthesizes high-quality speech from
articulatory signal in a multi-speaker situation. Most conventional
ATS approaches only focus on modeling contextual information
of speech from a single speaker’s articulatory features.
To explicitly represent each speaker’s speaking style as
well as the contextual information, our proposed model estimates
style embeddings, guided from the essential speech
style attributes such as pitch and energy. We adopt convolutional
layers and transformer-based attention layers for our
model to fully utilize both local and global information of articulatory
signals, measured by electromagnetic articulography
(EMA). Our model significantly improves the quality of
synthesized speech compared to the baseline in terms of objective
and subjective measurements in the Haskins dataset.

<br />

<h3>Samples
</h3>

<h4>Anger</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Text
        </td>
        <td class="text">
            두 사람 눈치 보기 싫어서 한 발이라도 먼저 나간다. (I don't want to look at them, so I'll take a step forward.)
        </td>
        <td class="text">
            아침 하기 싫어서 나오는 거 내 모를 줄 알아? (Don't you think I don't know you're coming out because you don't want to make breakfast?)
        </td>
        <td class="text">
            내 앞에 앉기 싫은 모양인데, 그럼 앉지마. (You don't want to sit in front of me, then don't sit down.)
        </td>
        <td class="text">
            들어오기 싫으면, 이참에 끝장을 내라고 그러세요. (If he don't want to come in, tell him to finish it this time.)
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/angry/anger_f_300.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/angry/angry_f_0750.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/angry/anger_m_161.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/angry/angry_m_0082.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/8_cer_base_anger_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/4_cer_base_angry_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/45_cer_base_anger_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/17_cer_base_angry_m2.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/8_prop_anger_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/4_prop_angry_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/45_prop_anger_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/angry/17_prop_angry_m2.wav"></audio></td>
    </tr>
</table>

 <h4>Happiness</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Text
        </td>
        <td class="text">
            난 아저씨가 빨리 우리 아빠가 됐으면 좋겠어. (I hope he will be my father soon.)
        </td>
        <td class="text">
            엿장수 맘대로 아니고, 지혜 맘대로. (It's not up to the candy seller, it's up to Jihye.)
        </td>
        <td class="text">
            그런 맘 먹기 힘들었을텐데, 고맙다 인경아. (It must have been hard for you to make up your mind, thank you In-kyung.)
        </td>
        <td class="text">
            아뇨, 전 호텔에서의 만찬보다는 이런 자리가 훨씬 편하고 좋은데요. (No, I like this kind of place much more comfortable than a hotel feast.)
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/happy/happy_f_422.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/happy/happy_f_0804.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/happy/happy_m_535.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/happy/happy_m_0088.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/4_cer_base_happy_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/13_cer_base_happy_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/10_cer_base_happy_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/28_cer_base_happy_m2.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/4_prop_happy_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/13_prop_happy_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/10_prop_happy_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/happy/28_prop_happy_m2.wav"></audio></td>
    </tr>
</table>

 <h4>Sadness</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Text
        </td>
        <td class="text">
            엄마가 날 안낳았다니까 더 우울하고 더 슬퍼. (It's even more depressing and sadder that my mom didn't give birth to me.)
        </td>
        <td class="text">
            나 아까워서 우리 혜인이 시집 못보내겠어. (I can't let my Hye-in get married because it's such a waste.)
        </td>
        <td class="text">
            오늘 만나면 어제 했던 말 취소한다고 할까봐 밤새 걱정했어. (When we met today, I was afraid you'd take back what you said yesterday.)
        </td>
        <td class="text">
            공휴일이라 쉬실텐데, 전화드려서 죄송합니다. (I'm sorry to call you because it's a public holiday.)
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/sad/sadness_f_709.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/sad/sad_f_1303.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/sad/sadness_m_581.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/sad/sad_m_0089.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/42_cer_base_sadness_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/2_cer_base_sad_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/27_cer_base_sadness_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/29_cer_base_sad_m2.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/42_prop_sadness_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/2_prop_sad_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/27_prop_sadness_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/sad/29_prop_sad_m2.wav"></audio></td>
    </tr>
</table>

 <h4>Neutral</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Text
        </td>
        <td class="text">
            세상에 둘도 없는 범생이 차림으로 갈 거다. (I'm going to dress up as the best student in the world.)
        </td>
        <td class="text">
            일본 작가가 쓴 소설을 출판하고 싶은가봐. (He seems to want to publish a novel written by a Japanese writer)
        </td>
        <td class="text">
            애한테 이런 불량식품을 사먹이면 어떡해요. (You shouldn't buy such junk food for that kid.)
        </td>
        <td class="text">
            아빠, 우리 유치원 얼마나 좋은데요. (Dad, my kindergarten is so nice.)
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/neutral/neutral_f_224.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/neutral/neutral_f_1818.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/neutral/neutral_m_746.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/ref/neutral/neutral_m_0122.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/16_cer_base__neutral_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/2_cer_base__neutral_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/48_cer_base__neutral_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/28_cer_base__neutral_m2.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/16_prop__neutral_f1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/2_prop__neutral_f2.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/48_prop__neutral_m1.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/neutral/28_prop__neutral_m2.wav"></audio></td>
    </tr>
</table>

<br />