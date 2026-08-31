---
permalink: /research/
layout: single
title: "Research"
header:
  overlay_image: /assets/images/research.jpg
  overlay_filter: 0.5
show_overlay_title: true
share: false
classes: wide
author_profile: false
---

<style>
/* no author sidebar on this page: let content use the full width */
.layout--single .page { width: 100%; padding-right: 0; }

/* Width is set site-wide via $max-width in main.scss, so the nav and hero stay
   the same width on every page. */

.research-areas { margin: 0; }

.research-area {
  display: flex;
  gap: 2.6rem;
  align-items: flex-start;
  margin: 0 0 3.4rem;
}
.research-area.reverse { flex-direction: row-reverse; }

/* stacked variant: text on top, figure below (full-width, centered) */
.research-area--stacked { display: block; }
.research-area--stacked .ra-figure { max-width: 900px; margin: 1.6rem auto 0; }

/* fda.jpg is portrait, so it grows tall fast; a narrower column keeps it from
   towering over a short text block. */
.ra-figure { flex: 0 0 46%; margin: 0; }
/* This row carries a figure and a video, so it can afford less width than the
   figure alone would take; the text column was down to ~360px at 72%. */
.ra-figure--lg { flex-basis: 62%; }
.ra-figure a { display: block; }
.ra-figure img {
  width: 100%;
  height: auto;
  border-radius: 10px;
  box-shadow: 0 6px 22px rgba(0,0,0,0.13);
  border: 1px solid #ececec;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.ra-figure a:hover img {
  transform: translateY(-3px);
  box-shadow: 0 12px 30px rgba(0,0,0,0.20);
}
.ra-credit {
  display: block;
  font-size: 0.82em;
  color: #6f767d;
  margin-top: 0.7em;
  line-height: 1.5;
}
.ra-credit .ra-cite { font-style: italic; color: #8a8f95; }

.ra-body { flex: 1 1 auto; }
.ra-body h3 {
  margin-top: 0;
  margin-bottom: 0.6em;
  padding-left: 0.7rem;
  border-left: 4px solid #3b9cba;
  line-height: 1.25;
}
.ra-body p { line-height: 1.65; }
.ra-pubs {
  margin-top: 0.9em;
  font-size: 0.93em;
  line-height: 1.7;
}
.ra-pubs .ra-pubs-label {
  display: inline-block;
  font-variant: small-caps;
  letter-spacing: 0.04em;
  font-weight: 700;
  color: #2c7a93;
  margin-right: 0.4em;
}
.ra-pubs a { font-weight: 600; }
/* The pointer to the full list is not a paper, so it takes the teal of the
   "Selected work" label and the heading rule instead of the blue used for
   every other link in the row. */
.ra-pubs a.ra-pubs-more { color: #2c7a93; }
.ra-pubs a.ra-pubs-more:hover { color: #1f5c70; }

.research-video {
  margin: 1.4rem 0 0;
}
.research-video .responsive-video-container {
  border-radius: 10px;
  box-shadow: 0 6px 22px rgba(0,0,0,0.13);
  margin-bottom: 0;
}

@media (max-width: 760px) {
  .research-area, .research-area.reverse { flex-direction: column; gap: 1.1rem; }
  .ra-figure { flex-basis: auto; width: 100%; }
}
</style>

<div class="research-areas">

  <section class="research-area">
    <div class="ra-figure ra-figure--lg">
      <a href="/assets/pdf/birds_citsci.pdf" target="_blank">
        <img src="/assets/images/research/conservation.jpg" alt="Seasonality patterns of four California bird species reconstructed separately from eBird and iNaturalist participatory science records">
      </a>
      <span class="ra-credit">Seasonality of four bird species reconstructed separately from eBird and iNaturalist records. The two platforms largely agree on the timing of each species. <span class="ra-cite">From Carroll et al., Citizen Science: Theory and Practice (2025).</span></span>
      <div class="research-video">
        <div class="responsive-video-container">
          <iframe src="https://www.youtube-nocookie.com/embed/pmHnEEVzpmI?vq=hd1080" frameborder="0" allowfullscreen></iframe>
        </div>
        <span class="ra-credit">UrchSearch Demo: Urchin Detection for Kelp Forest Restoration. <span class="ra-cite">From Lobo et al., The Nature Conservancy (2026).</span></span>
      </div>
    </div>
    <div class="ra-body">
      <h3>Conservation, citizen science, and biology</h3>
      <p>Much of my applied work has been in conservation and ecology, building automated tools for environmental monitoring and evaluating the data these fields rely on. With ecologists at UC Davis, I've validated participatory science data by comparing bird seasonality patterns across eBird and iNaturalist. Work with The Nature Conservancy has produced satellite-based monitoring workflows for field flooding, an automated pipeline to count sea urchins for kelp forest restoration monitoring, and large language models for accelerating groundwater sustainability plan reviews. Alongside these, I have maintained the NorCal Bird Dashboard, an interactive tool for exploring bird observation data across Northern California. Collaborations in biology have included studying neonatal survival in non-domestic Caprinae with veterinarians at the San Diego Zoo and the comparative biology of a groundwater isopod. Separately, I have worked with the researchers behind the Himalayan Database on what predicts success and survival for Mount Everest mountaineers.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Selected work</span>
        <a href="/assets/pdf/birds_citsci.pdf" target="_blank">eBird vs. iNaturalist Seasonality</a> (<em>Citizen Science: Theory and Practice</em>, 2025) ·
        <a href="/assets/pdf/llms_for_gsps.pdf" target="_blank">LLMs for Conservation Efficiency</a> (<em>Environmental Challenges</em>, 2026) ·
        <a href="/assets/pdf/isopods.pdf" target="_blank">Embryology and Transcriptomics of a Groundwater Isopod</a> (<em>Evolution &amp; Development</em>, 2025) ·
        <a href="/assets/pdf/everest.pdf" target="_blank">Mountaineers on Mount Everest</a> (<em>PLoS One</em>, 2020) ·
        <a href="/assets/pdf/tnc_urchins.pdf" target="_blank">Automated Sea Urchin Counting for Kelp Forest Restoration</a> (<em>The Nature Conservancy</em>, 2026) ·
        <a class="ra-pubs-more" href="/publications/">[Other Publications]</a>
      </p>
    </div>
  </section>

  <section class="research-area reverse">
    <div class="ra-figure">
      <a href="/assets/pdf/warpingsep.pdf" target="_blank">
        <img src="/assets/images/research/fda.jpg" alt="A latent deformation model that builds multivariate functional data from a shared latent process, warping each component onto its own time scale before producing the observed curves">
      </a>
      <span class="ra-credit">The latent deformation model assembles multivariate curves from a shared latent process, warping each component onto its own internal clock before the curves are observed. <span class="ra-cite">From Carroll and Müller, Biometrics (2023).</span></span>
    </div>
    <div class="ra-body">
      <h3>Biostatistics and functional data analysis</h3>
      <p>My methodological work has centered on functional and longitudinal data, particularly when the data involve multiple components or are subject to time warping. I have developed latent deformation models and cross-component registration methods for multivariate functional data, motivated by the study of human growth curves. These methods separate systematic phase variation, such as differences in the timing of growth spurts across individuals and across body measurements, from differences in amplitude. Beyond growth curves, I have applied the same tools to COVID-19, characterizing how case trajectories evolved across countries and forecasting case growth rates in the United States.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Selected work</span>
        <a href="/assets/pdf/warpingsep.pdf" target="_blank">Latent Deformation Models</a> (<em>Biometrics</em>, 2023) ·
        <a href="/assets/pdf/xcr.pdf" target="_blank">Cross-component Registration</a> (<em>Biometrics</em>, 2021) ·
        <a href="/assets/pdf/covid.pdf" target="_blank">Time Dynamics of COVID-19</a> (<em>Scientific Reports</em>, 2020) ·
        <a href="/assets/pdf/covid_delay.pdf" target="_blank">Learning Delay Dynamics for COVID-19 Growth</a> (<em>J. Math. Anal. Appl.</em>, 2022) ·
        <a href="https://cran.r-project.org/web/packages/fdapace/index.html" target="_blank">fdapace R package</a> ·
        <a class="ra-pubs-more" href="/publications/">[Other Publications]</a>
      </p>
    </div>
  </section>

  <section class="research-area research-area--stacked">
    <div class="ra-body">
      <h3>Statistical modeling of healthcare data</h3>
      <p>On the biomedical side, my collaborations have spanned vision, hearing, cancer, and mental health. ABRA, an open-source deep learning toolbox for automated auditory brainstem response analysis, has come out of a collaboration with auditory researchers in the <a href="https://manorlab.ucsd.edu/" target="_blank">Manor Lab</a> at UC San Diego. At UCSF, I have studied kinase signaling in cancer with Hui Lin and Jean-Philippe Coppé, using graph neural networks and protein language model embeddings to identify the kinases that drive resistance to treatment. A separate project with the <a href="http://capralab.org/" target="_blank">Capra Lab</a> has applied protein language models, treating protein sequences as text to predict how mutations affect protein function. For the <a href="https://ketamineresearchfoundation.org/" target="_blank">Ketamine Research Foundation</a>, I have traced longitudinal change in depression and anxiety among adolescents and young adults receiving ketamine-assisted psychotherapy. Ophthalmologists at Stanford Medicine and I have used statistical and machine learning methods to predict progressive vision loss in glaucoma patients from electronic health records.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Selected work</span>
        <a href="https://doi.org/10.1038/s41598-026-38045-1" target="_blank">ABRA Deep Learning Toolbox</a> (<em>Scientific Reports</em>, 2026) ·
        <a href="https://www.frontiersin.org/articles/10.3389/fpsyt.2026.1886833/abstract" target="_blank">Ketamine-Assisted Psychotherapy in Youth</a> (<em>Frontiers in Psychiatry</em>, in press) ·
        <a href="/assets/pdf/fpca_glaucoma.pdf" target="_blank">FPCA for Glaucoma Progression</a> (<em>Frontiers in Ophthalmology</em>, 2025) ·
        <a href="/assets/pdf/dvh.pdf" target="_blank">Knowledge-Based DVH Prediction</a> (<em>J. Appl. Clin. Med. Phys.</em>, 2021) ·
        <a class="ra-pubs-more" href="/publications/">[Other Publications]</a>
      </p>
    </div>
    <div class="ra-figure ra-figure--lg">
      <a href="/assets/pdf/abra.pdf" target="_blank">
        <img src="/assets/images/research/health.jpg" alt="Auditory brainstem response waveforms analyzed across sound levels, with automated peak detection and hearing threshold estimation">
      </a>
      <span class="ra-credit">ABR waveforms analyzed across sound levels, with automated peak detection and threshold estimation. The hearing threshold is the lowest level at which a response is still detectable. <span class="ra-cite">From Erra et al., Scientific Reports (2026).</span></span>
    </div>
  </section>

</div>

A full list of my publications can be found on my <a href="https://scholar.google.com/citations?user=EY7x1lYAAAAJ&hl=en" target="_blank">Google Scholar profile</a>.
