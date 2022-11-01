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
<img src="./assets/img/Proposed_v5.png" width="400">

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

<h3>Samples per speakers
</h3>

 <h4>Female (F03)</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Text
        </td>
        <td class="text">
            Two blue fish swam in the tank. 
        </td>
        <td class="text">
            The ink stain dried on the finished page.
        </td>
        <td class="text">
            The young kid jumped the rusty gate.
        </td>
        <td class="text">
            This plank was made for walking on.
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B01_S26_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B02_S13_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B03_S21_R02_N_target.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B07_S07_R01_N_target.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Baseline</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B01_S26_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B02_S13_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B03_S21_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/baseline/F03_B07_S07_R01_N.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Proposed</td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B01_S26_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B02_S13_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B03_S21_R02_N.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/Samples_demo/F03/F03_B07_S07_R01_N.wav"></audio></td>
    </tr>
</table>


 <h4>Male (M03)</h4>

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