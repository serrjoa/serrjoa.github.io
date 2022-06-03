---
layout: page
title: UNIVERSE
---

# Universal Speech Enhancement With Score-based Diffusion

This is the companion page of UNIVERSE, the universal speech enhancer described in the paper "Universal Speech Enhancement With Score-based Diffusion" by Joan Serrà, Santiago Pascual, Jordi Pons, R. Oguz Araz, and Davide Scaini. To access the paper, click [here]().

## Info

### Abstract

Removing background noise from speech audio has been the subject of considerable research and effort, especially in recent years due to the rise of virtual communication and amateur sound recording. Yet background noise is not the only unpleasant disturbance that can prevent intelligibility: reverb, clipping, codec artifacts, problematic equalization, limited bandwidth, or inconsistent loudness are equally disturbing and ubiquitous. In this work, we propose to consider the task of speech enhancement as a holistic endeavor, and present a universal speech enhancement system that tackles 55 different distortions at the same time. Our approach consists of a generative model that employs score-based diffusion, together with a multi-resolution conditioning network that performs enhancement with mixture density networks. We show that this approach significantly outperforms the state of the art in a subjective test performed by expert listeners. We also show that it achieves competitive objective scores with just 4-8 diffusion steps, despite not considering any particular strategy for fast sampling. We hope that both our methodology and technical contributions encourage researchers and practitioners to adopt a universal approach to speech enhancement, possibly framing it as a generative task.

### Reference

> **Universal Speech Enhancement With Score-based Diffusion** <br>
> J. Serrà, S. Pascual, J. Pons, R. O. Araz, & D. Scaini. <br>
> *Preprint*. June 2022.

### Core idea

The next video highlights the core idea of the project.

<div style="text-align: center"><iframe src="https://player.vimeo.com/video/713702603?h=47bb673343&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="talk-1d-540p"></iframe></div>

## Examples

Here we provide a number of examples of enhancements performed by UNIVERSE. There are three sections: (1) examples enhancing the speech in real-world videos, (2) examples enhancing real-world speech recordings, and (3) examples from our validation set highlighting the removal of different and often simultaneous distortions.

### Real-world speech from video

*\[Sources: [Internet Archive](https://archive.org/) and [Youtube](https://www.youtube.com/) | License: Creative Commons (see videos)\]*

**Documentaries** &mdash; In old documentaries, the speech voice is usually band limited and dynamically compressed. In addition, recordings can also contain some background noise or codec artifacts due to suboptimal recording or digitization, respectively. Clipping or reverb may also be not in full control.

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702342?h=0fe536dcff&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="documentary-1-540p"></iframe></div>

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702407?h=4d7f0604f3&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="documentary-2-540p"></iframe></div>

**Talks** &mdash; Talks given in class or conference rooms typically contain a large amount of reverberation. In addition, they feature inconsistent loudness levels and problematic equalization depending on the distance and angle between the speaker and the microphone. Some background noise can also be present.

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702555?h=221b93cbb6&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="talk-1b-540p"></iframe></div>

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702531?h=d0bb60e9d6&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="talk-4-540p"></iframe></div>

**Cooking** &mdash; Cooking is a good example of a noisy environment where, sometimes, a distant microphone is placed to record the mixture with speech. In many cases, post-production background music is also added, and some amount of natural or synthetic reverberation can be present.

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702311?h=3e0a6c119a&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="cooking-2-540p"></iframe></div>

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702260?h=ec83d7703a&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="cooking-1-540p"></iframe></div>

**Other** &mdash; Other example situations where speech recordings may contain some distortion are in room recordings with a distant microphone, exterior recordings featuring background noise, or recordings done with non-professional means. In addition, audio may be encoded with an aggressive compression factor, yielding a series of codec artifacts.

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702449?h=92dd8404de&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="sketch-1-540p"></iframe></div>

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702644?h=3f2aab7bb4&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="tourism-1-540p"></iframe></div>

<div style="text-align: left"><iframe src="https://player.vimeo.com/video/713702479?h=4db26f9c57&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="480" height="270" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen title="sports-1-540p"></iframe></div>

### Real-world speech recordings

*\[Source: [Freesound](https://freesound.org/) | License: Creative Commons [CC-0-1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.en)\]*

**Background noise** &mdash; Here we remove background noise under different SNRs.

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/328842__deleted-user-958643__hey-give-it-back.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/328842__deleted-user-958643__hey-give-it-back.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/401794__sean-te0__we-ll-eat-pizzas.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/401794__sean-te0__we-ll-eat-pizzas.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Reverb** &mdash; Here we have examples of a room reverb that is removed.

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/87644__alcoceba__frase.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/87644__alcoceba__frase.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/450205__miguelgc96__speech-camaron.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/450205__miguelgc96__speech-camaron.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Clipping/dynamics** &mdash; This is an example of controling the dynamic range and removing some clipping.

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/345857__lakethepondling__batman.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/345857__lakethepondling__batman.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Expressivity** &mdash; Here is an example to show that, despite being a generative model, UNIVERSE does not loose expressivity in the enhancement process.

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/31755__streety__globalwarming.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/31755__streety__globalwarming.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Deessing** &mdash; This example shows that the model also controls strong sibilant sounds.

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/619322__unfa__de-esser-stress-test_input.in.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_freesound/619322__unfa__de-esser-stress-test_input.out.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

### Validation set utterances

*\[Sources: Publicly-available data sets (see paper) | License: Creative Commons [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.en)\]*

**Silent gaps**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0001_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0001_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Codec + Dynamics + EQ + Noise + Spectral manipulation**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0016_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0016_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Noise + Reverb**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0018_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0018_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Noise + High-pass**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0030_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0030_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Codec + Clipping**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0035_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0035_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Low-pass**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0039_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0039_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Telephonic speech + Dynamics compressor**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0044_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0044_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Noise + Codec**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0045_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0045_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**Noise + Silent gaps**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0056_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0056_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

**EQ + Reverb**

<table style="width:480">
  <tbody>
    <tr>
      <td>
        Input:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0062_xd.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
    <tr>
      <td>
        Enhanced:
      </td>
      <td>
        <html>
          <audio controls>
            <source src="audio_validation/0062_xe.wav" type="audio/wav">
          </audio>
        </html>
      </td>
    </tr>
  </tbody>
</table>

## Validation subset download

To foster further subjective evaluation, we provide the first (random) 100 utterances of our validation data [here](https://dolby.box.com/s/mq5uxiv0rmo2nqbi3gxhrke87lngpn0e). Input, target, and enhanced files are included, together with a small description of speech/noise sources and applied distortions.

<br>
<br>

<div style="text-align: right"><i>[Last edit: June 2022]</i></div>
