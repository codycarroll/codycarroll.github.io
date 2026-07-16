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

/* widen the overall content area on this page so the text column isn't cramped */
#main { max-width: 1500px; }
/* widen the top nav bar and header title to match the wider content */
.masthead__inner-wrap { max-width: 1500px; }
.page__hero--overlay .wrapper { max-width: 1500px; }

.research-areas { margin: 0; }

.research-area {
  display: flex;
  gap: 2.6rem;
  align-items: flex-start;
  margin: 0 0 3.4rem;
}
.research-area.reverse { flex-direction: row-reverse; }

.ra-figure { flex: 0 0 56%; margin: 0; }
.ra-figure--lg { flex-basis: 66%; }
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
    <div class="ra-figure">
      <a href="/assets/pdf/warpingsep.pdf" target="_blank">
        <img src="/assets/images/research/fda.jpg" alt="A latent deformation model that builds multivariate functional data from a shared latent process, warping each component onto its own time scale before producing the observed curves">
      </a>
      <span class="ra-credit">The latent deformation model assembles multivariate curves from a shared latent process, warping each component onto its own internal clock before the curves are observed. <span class="ra-cite">From C. and Müller, Biometrics (2023).</span></span>
    </div>
    <div class="ra-body">
      <h3>Functional and longitudinal data analysis</h3>
      <p>Much of my methodological work focuses on functional and longitudinal data, particularly when the data involve multiple components or are subject to time warping. I developed latent deformation models and cross-component registration methods for multivariate functional data, motivated by the study of human growth curves. These methods separate systematic phase variation, such as differences in the timing of growth spurts across individuals and across body measurements, from differences in amplitude. During the COVID-19 pandemic, I applied functional data methods to characterize how case trajectories evolved across countries and to forecast case growth rates in the United States.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Key works</span>
        <a href="/assets/pdf/warpingsep.pdf" target="_blank">Latent Deformation Models</a> (<em>Biometrics</em>, 2023) ·
        <a href="/assets/pdf/xcr.pdf" target="_blank">Cross-component Registration</a> (<em>Biometrics</em>, 2021) ·
        <a href="/assets/pdf/covid.pdf" target="_blank">Time Dynamics of COVID-19</a> (<em>Scientific Reports</em>, 2020) ·
        <a href="/assets/pdf/covid_delay.pdf" target="_blank">Learning Delay Dynamics for COVID-19 Growth</a> (<em>J. Math. Anal. Appl.</em>, 2022) ·
        <a href="https://cran.r-project.org/web/packages/fdapace/index.html" target="_blank">fdapace R package</a>
      </p>
    </div>
  </section>

  <section class="research-area reverse">
    <div class="ra-figure ra-figure--lg">
      <a href="/assets/pdf/birds_citsci.pdf" target="_blank">
        <img src="/assets/images/research/conservation.jpg" alt="Seasonality patterns of four California bird species reconstructed separately from eBird and iNaturalist participatory science records">
      </a>
      <span class="ra-credit">Seasonality of four bird species reconstructed separately from eBird and iNaturalist records. The two platforms largely agree on the timing of each species. <span class="ra-cite">From C. et al., Citizen Science: Theory and Practice (2025).</span></span>
      <div class="research-video">
        <div class="responsive-video-container">
          <iframe src="https://www.youtube-nocookie.com/embed/pmHnEEVzpmI?vq=hd1080" frameborder="0" allowfullscreen></iframe>
        </div>
        <span class="ra-credit">UrchSearch Demo: Urchin Detection for Kelp Forest Restoration. <span class="ra-cite">From Lobo et al., The Nature Conservancy (2026).</span></span>
      </div>
    </div>
    <div class="ra-body">
      <h3>Conservation, citizen science, and biology</h3>
      <p>I work with conservation scientists at The Nature Conservancy and UC Davis. Current projects include validating participatory science data by comparing bird seasonality patterns across eBird and iNaturalist, developing satellite-based monitoring workflows for field flooding, building an automated pipeline to count sea urchins for kelp forest restoration monitoring, and using large language models to accelerate groundwater sustainability plan reviews. I also maintain the NorCal Bird Dashboard, an interactive tool for exploring bird observation data across Northern California. My collaborations in biology include neonatal survival in non-domestic Caprinae with veterinarians at the San Diego Zoo, the comparative biology of a groundwater isopod, and the determinants of success and survival for Mount Everest mountaineers.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Key works</span>
        <a href="/assets/pdf/birds_citsci.pdf" target="_blank">eBird vs. iNaturalist Seasonality</a> (<em>Citizen Science: Theory and Practice</em>, 2025) ·
        <a href="/assets/pdf/llms_for_gsps.pdf" target="_blank">LLMs for Conservation Efficiency</a> (<em>Environmental Challenges</em>, 2026) ·
        <a href="/assets/pdf/goats.pdf" target="_blank">Neonatal Survivability in Non-Domestic Caprinae</a> (<em>Journal of Zoo and Wildlife Medicine</em>, 2022) ·
        <a href="/assets/pdf/isopods.pdf" target="_blank">Embryology and Transcriptomics of a Groundwater Isopod</a> (<em>Evolution &amp; Development</em>, 2025) ·
        <a href="/assets/pdf/everest.pdf" target="_blank">Mountaineers on Mount Everest</a> (<em>PLoS One</em>, 2020) ·
        <a href="https://birds-dash-547zxcr6ea-uc.a.run.app/" target="_blank">NorCal Bird Dashboard</a> ·
        <a href="/assets/pdf/tnc_birdsense.pdf" target="_blank">Satellite Monitoring of Field Flooding</a> (<em>The Nature Conservancy</em>, 2023) ·
        <a href="/assets/pdf/tnc_urchins.pdf" target="_blank">Automated Sea Urchin Counting for Kelp Forest Restoration</a> (<em>The Nature Conservancy</em>, 2026)
      </p>
    </div>
  </section>

  <section class="research-area">
    <div class="ra-figure ra-figure--lg">
      <a href="/assets/pdf/abra.pdf" target="_blank">
        <img src="/assets/images/research/health.jpg" alt="Auditory brainstem response waveforms analyzed across sound levels, with automated peak detection and hearing threshold estimation">
      </a>
      <span class="ra-credit">ABR waveforms analyzed across sound levels, with automated peak detection and threshold estimation. The hearing threshold is the lowest level at which a response is still detectable. <span class="ra-cite">From Erra et al., Scientific Reports (2026).</span></span>
      <a href="/assets/pdf/fpca_glaucoma.pdf" target="_blank" style="margin-top: 1.4rem;">
        <img src="/assets/images/research/health2.jpg" alt="Predicted visual field trajectories for sample fast and slow glaucoma progressors, and scatterplots of actual versus predicted mean deviation colored by prediction horizon">
      </a>
      <span class="ra-credit">Predicted visual field trajectories for sample fast and slow glaucoma progressors (top), with actual versus predicted mean deviation across prediction horizons (bottom). <span class="ra-cite">From Donnipadu et al., Frontiers in Ophthalmology (2025).</span></span>
    </div>
    <div class="ra-body">
      <h3>Statistical modeling of healthcare data</h3>
      <p>On the biomedical side, I work with ophthalmologists at Stanford Medicine on predicting progressive vision loss in glaucoma patients from electronic health records, using statistical and machine learning methods. I also collaborate with auditory researchers in the <a href="https://manorlab.ucsd.edu/" target="_blank">Manor Lab</a> at UC San Diego, where our team developed ABRA, an open-source deep learning toolbox for automated auditory brainstem response analysis. At UCSF, I work with Hui Lin and Jean-Philippe Coppé on kinase signaling in cancer, using graph neural networks and protein language model embeddings to identify the kinases that drive resistance to treatment. Separately, I collaborate with the <a href="http://capralab.org/" target="_blank">Capra Lab</a> in epidemiology and biostatistics. I also work with the <a href="https://ketamineresearchfoundation.org/" target="_blank">Ketamine Research Foundation</a>, characterizing longitudinal change in depression and anxiety among adolescents and young adults receiving ketamine-assisted psychotherapy.</p>
      <p class="ra-pubs"><span class="ra-pubs-label">Key works</span>
        <a href="https://doi.org/10.1038/s41598-026-38045-1" target="_blank">ABRA Deep Learning Toolbox</a> (<em>Scientific Reports</em>, 2026) ·
        <a href="/assets/pdf/fpca_glaucoma.pdf" target="_blank">FPCA for Glaucoma Progression</a> (<em>Frontiers in Ophthalmology</em>, 2025) ·
        <a href="/assets/pdf/dvh.pdf" target="_blank">Knowledge-Based DVH Prediction</a> (<em>J. Appl. Clin. Med. Phys.</em>, 2021)
      </p>
    </div>
  </section>

</div>

A full list of my publications can be found on my <a href="https://scholar.google.com/citations?user=EY7x1lYAAAAJ&hl=en" target="_blank">Google Scholar profile</a>.
