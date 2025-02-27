<div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://pepy.tech/badge/syft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies-run.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies-run.yml/badge.svg?branch=dev" /></a> <a href="https://gitpod.io/#https://github.com/OpenMined/PySyft"><img src="https://img.shields.io/badge/gitpod-908a85?logo=gitpod" /></a>
<a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
<br /><br /></div>

<img src="packages/syft/docs/img/title_syft_light.png#gh-light-mode-only" alt="Syft Logo" width="200px" />
<img src="packages/syft/docs/img/title_syft_dark.png#gh-dark-mode-only" alt="Syft Logo" width="200px" />

Perform `numpy`-like analysis on `data` that remains in `someone else's` server

<div align="left">
<img src="packages/syft/docs/img/header.png#gh-light-mode-only" alt="Syft Overview" width="100%" />
<img src="packages/syft/docs/img/header.png#gh-dark-mode-only" alt="Syft Overview" width="100%" />
</div>

# Quickstart

✅ `Linux` ✅ `macOS`\* ✅ `Windows`†‡
<img src="packages/syft/docs/img/terminalizer.gif" width="50%" align="right" />

1. Install our handy 🛵 cli tool which makes deploying a Domain or Network server a one-liner:  
   `pip install -U hagrid`

2. Then run our interactive jupyter Install 🧙🏽‍♂️ Wizard<sup>BETA</sup>:  
   `hagrid quickstart`

- In the tutorial you will learn how to install and deploy:  
  `PySyft` = our `numpy`-like 🐍 Python library for computing on `private data` in someone else's `Domain`

  `PyGrid` = our 🐳 `docker` / `k8s` / 🐧 `vm` `Domain` & `Network` Servers where `private data` lives

- During quickstart we will deploy `PyGrid` to localhost with 🐳 `docker`, however 🛵 HAGrid can deploy to `k8s` or a 🐧 `ubuntu` VM on `azure` / `gcp` / `ANY_IP_ADDRESS` by using 🔨 `ansible`†

3. Read our 📚 <a href="https://openmined.github.io/PySyft/">Docs</a>
4. Ask Questions ❔ in `#support` on <a href="https://slack.openmined.org/">Slack</a>

# Install Notes

- HAGrid Requires: 🐍 `python` 🐙 `git` - Run: `pip install -U hagrid`
- Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`  
  †`Windows` does not support `ansible`, preventing some remote deployment targets
- PySyft Requires: 🐍 `python 3.7+` - Run: `pip install -U syft --pre`  
  \*`macOS` Apple Silicon users need cmake: `brew install cmake`  
  ‡`Windows` users must run this first: `pip install jaxlib==0.3.14 -f https://whls.blob.core.windows.net/unstable/index.html`
- PyGrid Requires: 🐳 `docker` / `k8s` or 🐧 `ubuntu` VM - Run: `hagrid launch ...`

# Versions

<!-- `0.8.0 beta` - `dev` branch 👈🏽   -->

`0.7.0 beta` - `dev` branch 👈🏽  
`0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>  
`0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix  
`0.2.0` - `0.5.0` Deprecated

PySyft and PyGrid use the same `version` and its best to match them up where possible. We release weekly betas which can be used in each context:
PySyft: `pip install -U syft --pre`
PyGrid: `hagrid launch ... tag=latest`

<!-- Quickstart: `hagrid quickstart --pre` -->

HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.

# What is Syft?

<img align="right" src="packages/syft/docs/img/logo_big.png#gh-light-mode-only" alt="Syft" height="250" style="padding-left:30px;">

<img align="right" src="packages/syft/docs/img/logo_big_dark.png#gh-dark-mode-only" alt="Syft" height="250" style="padding-left:30px;">

`Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.

### Why should I use Syft?

`Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.

No more cold calls to get `access` to a dataset. No more weeks of `wait times` to get a `result` on your `query`. It also means `1000x more data` in every domain. PySyft opens the doors to a streamlined Data Scientist `workflow`, all with the individual's `privacy` at its heart.

# Tutorials

<table border="5" bordercolor="grey">
<tr>
<th align="center">
<img width="441" height="1">
<div align="center">
<img src="packages/syft/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
<p>Data Owner</p></div>
</th>
<th align="center">
<img width="441" height="1">
<div align="center"><img src="packages/syft/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
<p>Data Scientist</p></div>

</th>
<th align="center">
<img width="441" height="1">
<div align="center">
<img src="packages/syft/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
<p>Data Engineer</p>
</div>
</th>
</tr>
<tr>
<td valign="top">

- <a href="/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
- <a href="/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
- Create Accounts</a>
- Manage Privacy Budget</a>
- Join a Network</a>
- Learn how PETs streamline Data Policies

</td>
<td valign="top">

- Install Syft</a>
- Connect to a Domain</a>
- Search for Datasets</a>
- Train Models
- Retrieve Secure Results
- Learn Differential Privacy

</td>
<td valign="top">

- Setup Dev Mode</a>
- Deploy to Azure
- Deploy to GCP
- Deploy to Kubernetes
- Customize Networking
- Modify PyGrid UI
</td>
</tr>
</table>

# Terminology

<table border="5" bordercolor="grey">
<tr>
<th align="center">
<img width="441" height="1">
<p>👨🏻‍💼 Data Owners</p>
</th>
<th align="center">
<img width="441" height="1">
<p>👩🏽‍🔬 Data Scientists</p>
</th>
</tr>
<tr>
<td valign="top">
<!-- REMOVE THE BACKSLASHES -->

Provide `datasets` which they would like to make available for `study` by an `outside party` they may or may not `fully trust` has good intentions.

</td>
<td valign="top">
<!-- REMOVE THE BACKSLASHES -->

Are end `users` who desire to perform `computations` or `answer` a specific `question` using one or more data owners' `datasets`.

</td>
</tr>
<tr>
<th align="center">
<img width="441" height="1">
<p>🏰 Domain Server</p>
</th>
<th align="center">
<img width="441" height="1">
<p>🔗 Network Server</p>
</th>
</tr>
<tr>
<td valign="top">
<!-- REMOVE THE BACKSLASHES -->

Manages the `remote study` of the data by a `Data Scientist` and allows the `Data Owner` to manage the `data` and control the `privacy guarantees` of the subjects under study. It also acts as a `gatekeeper` for the `Data Scientist's` access to the data to compute and experiment with the results.

</td>
<td valign="top">
<!-- REMOVE THE BACKSLASHES -->

Provides services to a group of `Data Owners` and `Data Scientists`, such as dataset `search` and bulk `project approval` (legal / technical) to participate in a project. A network server acts as a bridge between it's members (`Domains`) and their subscribers (`Data Scientists`) and can provide access to a collection of `domains` at once.</td>

</tr>
<tr>
</table>

# Community

<table border="5" bordercolor="grey">
<tr>
<th align="center" valign="top">
<img width="441" height="1">
<div align="center">
<img src="packages/syft/docs/img/panel_slack_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
<img src="packages/syft/docs/img/panel_slack_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />

<a href="https://slack.openmined.org/"><img src="packages/syft/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>

</div>
</th>
<th align="center" valign="top">
<img width="441" height="1">
<div align="center">
<img src="packages/syft/docs/img/panel_title_videos_papers_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
<img src="packages/syft/docs/img/panel_title_videos_papers.png#gh-dark-mode-only" alt="" width="100%" align="center" />
<p align="left"><sub><sup>
🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
🎥 <a href="https://www.youtube.com/watch?v=NJBBE_SN90A">Privacy Preserving AI - PyTorch Devcon 2019</a><br />
📖 <a href="https://arxiv.org/pdf/2110.01315.pdf">Towards general-purpose infrastructure for protect...</a><br />
📖 <a href="https://arxiv.org/pdf/2104.12385.pdf">Syft 0.5: A platform for universally deployable ...</a><br />
📖 <a href="https://arxiv.org/pdf/1811.04017.pdf">A generic framework for privacy preserving deep ...</a>
</sup></sup></p>
</div>
</th>
<th align="center" valign="top">
<img width="441" height="1">
<div align="center">
<img src="packages/syft/docs/img/panel_padawan_title_light.png#gh-light-mode-only" alt="" width="100%" align="center" />
<img src="packages/syft/docs/img/panel_padawan_title_dark.png#gh-dark-mode-only" alt="" width="100%" align="center" />

<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="packages/syft/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>

</div>
</th>
</tr>
</table>

# Courses

<table border="5" bordercolor="grey">
<tr>
<th align="center">
<img width="441" height="1">
<div align="center">
<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="packages/syft/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
</th>
<th align="center">
<img width="441" height="1">
<div align="center">
<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="packages/syft/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
</div>
</th>
<th align="center">
<img width="441" height="1">
<div align="center">
<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="packages/syft/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
</div>
</th>
</tr>
</table>

# Contributors

OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />  
<img src="packages/syft/docs/img/contributors_light.jpg#gh-light-mode-only" alt="Contributors" width="100%" />
<img src="packages/syft/docs/img/contributors_dark.jpg#gh-dark-mode-only" alt="Contributors" width="100%" />

# Supporters

<table border="0">
<tr>
<th align="center">
<a href="https://sloan.org/"><img src="packages/syft/docs/img/logo_sloan.png" /></a>
</th>
<th align="center">
<a href="https://opensource.fb.com/"><img src="packages/syft/docs/img/logo_meta.png" /></a>
</th>
<th align="center">
<a href="https://pytorch.org/"><img src="packages/syft/docs/img/logo_torch.png" /></a>
</th>
<th align="center">
<a href="https://www.udacity.com/"><img src="packages/syft/docs/img/logo_udacity.png" /></a>
</th>
<th align="center">
<a href="https://summerofcode.withgoogle.com/"><img src="packages/syft/docs/img/logo_gsoc.png" /></a>
</th>
<th align="center">
<a href="https://developers.google.com/season-of-docs"><img src="packages/syft/docs/img/logo_gsod.png" /></a>
</th>
<th align="center">
<img src="packages/syft/docs/img/logo_arkhn_light.png#gh-light-mode-only" />
<img src="packages/syft/docs/img/logo_arkhn.png#gh-dark-mode-only" />
</th>
<th align="center">
<img src="packages/syft/docs/img/logo_cape_light.png#gh-light-mode-only" />
<img src="packages/syft/docs/img/logo_cape.png#gh-dark-mode-only" />
</th>
<th align="center">
<a href="https://begin.ai/"><img src="packages/syft/docs/img/logo_begin.png" /></a>
</th>
</tr>
</table>

# Open Collective

`OpenMined` is a registered `501(c)(3)` in the USA. We are funded by our gracious supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
<img src="packages/syft/docs/img/opencollective_light.png#gh-light-mode-only" alt="Contributors" width="100%" />
<img src="packages/syft/docs/img/opencollective_dark.png#gh-dark-mode-only" alt="Contributors" width="100%" />

# Disclaimer

Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.

# License

[Apache License 2.0](LICENSE)<br />
<a href="https://www.flaticon.com/free-icons/person" title="person icons">Person icons created by Freepik - Flaticon</a>


<table border="0">
<tr>
<th align="center">
<a href="https://sloan.org/"><img src="packages/syft/docs/img/logo_sloan.png" /></a>
</th>
<th align="center">
<a href="https://opensource.fb.com/"><img src="packages/syft/docs/img/logo_meta.png" /></a>
</th>
<th align="center">
<a href="https://pytorch.org/"><img src="packages/syft/docs/img/logo_torch.png" /></a>
</th>
<th align="center">
<a href="https://www.udacity.com/"><img src="packages/syft/docs/img/logo_udacity.png" /></a>
</th>
<th align="center">
<a href="https://summerofcode.withgoogle.com/"><img src="packages/syft/docs/img/logo_gsoc.png" /></a>
</th>
<th align="center">
<a href="https://developers.google.com/season-of-docs"><img src="packages/syft/docs/img/logo_gsod.png" /></a>
</th>
<th align="center">
<img src="packages/syft/docs/img/logo_arkhn_light.png#gh-light-mode-only" />
<img src="packages/syft/docs/img/logo_arkhn.png#gh-dark-mode-only" />
</th>
<th align="center">
<img src="packages/syft/docs/img/logo_cape_light.png#gh-light-mode-only" />
<img src="packages/syft/docs/img/logo_cape.png#gh-dark-mode-only" />
</th>
<th align="center">
<a href="https://begin.ai/"><img src="packages/syft/docs/img/logo_begin.png" /></a>
</th>
</tr>
</table>