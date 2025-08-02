---
title: "Meet the Researchers"
---

We are a collaborative team from EPFL and ETH Zürich working as part of the [Swiss AI Initiative](https://www.swiss-ai.org/).

<style>
.team-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1em;
    margin: 2em 0;
}

@media (max-width: 1200px) {
    .team-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

@media (max-width: 900px) {
    .team-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 600px) {
    .team-grid {
        grid-template-columns: 1fr;
    }
}

.team-member {
    text-align: center;
    padding: 1.5em;
    background: var(--entry);
    border-radius: 8px;
    border: 1px solid var(--border);
    position: relative;
    transition: all 0.3s ease;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.team-member:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.team-member img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 1em;
    border: 3px solid var(--border);
}

.team-member h3 {
    margin: 0.5em 0;
    font-size: 1.0em;
    color: var(--primary);
}

.team-member .affiliation {
    color: var(--secondary);
    font-size: 0.9em;
    margin: 0.3em 0;
}

.team-member .email-link {
    position: absolute;
    bottom: 5px;
    left: 50%;
    transform: translateX(-50%);
    background: #1a1a1a;
    color: #ffffff;
    padding: 0.3em 0.8em;
    border-radius: 20px;
    font-size: 0.75em;
    text-decoration: none;
    opacity: 0;
    transition: opacity 0.3s ease;
    white-space: nowrap;
}

.team-member:hover .email-link {
    opacity: 1;
}

.team-member .email-link:hover {
    background: #000000;
}

.supervisor-note {
    font-size: 0.9em;
    color: var(--secondary);
    text-align: center;
    margin: 2em 0;
}

/* Center the last team member when it's alone in the row */
.team-grid .team-member:nth-child(7) {
    grid-column: 2;
}

/* Responsive centering for smaller screens */
@media (max-width: 900px) {
    .team-grid .team-member:nth-child(7) {
        grid-column: 1; /* Reset to normal flow on 2-column layout */
    }
}

@media (max-width: 600px) {
    .team-grid .team-member:nth-child(7) {
        grid-column: 1; /* Reset to normal flow on 1-column layout */
    }
}

/* Dark mode specific adjustments */
@media (prefers-color-scheme: dark) {
    .dark .team-member {
        background: var(--entry);
    }
    
    .dark .team-member:hover {
        box-shadow: 0 5px 15px rgba(255,255,255,0.1);
    }
}
</style>

<div class="team-grid">

<div class="team-member">
<img src="/authors/Dongyang.png" alt="Dongyang Fan">
<h3>Dongyang Fan</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:dongyang.fan@epfl.ch" class="email-link">dongyang.fan@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/vinko.jpg" alt="Vinko Sabolčec">
<h3>Vinko Sabolčec</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:vinko.sabolcec@epfl.ch" class="email-link">vinko.sabolcec@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/matin.jpg" alt="Matin Ansaripour">
<h3>Matin Ansaripour</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:matin.ansaripour@epfl.ch" class="email-link">matin.ansaripour@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/Ayush.jpg" alt="Ayush Kumar Tarun">
<h3>Ayush Kumar Tarun</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:ayush.tarun@epfl.ch" class="email-link">ayush.tarun@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/Martin.jpeg" alt="Martin Jaggi">
<h3>Martin Jaggi</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:martin.jaggi@epfl.ch" class="email-link">martin.jaggi@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/antoine.jpg" alt="Antoine Bosselut">
<h3>Antoine Bosselut</h3>
<div class="affiliation">EPFL</div>
<a href="mailto:antoine.bosselut@epfl.ch" class="email-link">antoine.bosselut@epfl.ch</a>
</div>

<div class="team-member">
<img src="/authors/imanol.jpeg" alt="Imanol Schlag">
<h3>Imanol Schlag</h3>
<div class="affiliation">ETH Zürich</div>
<a href="mailto:ischlag@ethz.ch" class="email-link">ischlag@ethz.ch</a>
</div>

</div>


## 📧 Contact

For questions about our research, tools, or datasets, please contact [dongyang.fan@epfl.ch](mailto:dongyang.fan@epfl.ch).



## Acknowledgments

We gratefully acknowledge the support of:
- Swiss National Science Foundation (No. 215390)
- Innosuisse (PFFS-21-29)
- EPFL Center for Imaging
- Sony Group Corporation
- Meta LLM Evaluation Research Grant
- Swiss National Supercomputing Centre (CSCS) under project ID a06 on Alps


<div style="display: flex; justify-content: center; align-items: center; gap: 3em; margin: 2em 0; padding: 2em; background-color: var(--tertiary); border-radius: 8px;">
<a href="https://www.swiss-ai.org/" target="_blank" style="display: flex; align-items: center; justify-content: center; width: 200px; height: 100px; text-decoration: none !important; border: none !important; box-shadow: none !important;">
<img src="/logos/swissai.png" alt="Swiss AI Initiative" style="max-width: 100%; max-height: 100%; object-fit: contain;">
</a>
<a href="https://www.epfl.ch/" target="_blank" style="display: flex; align-items: center; justify-content: center; width: 200px; height: 100px; text-decoration: none !important; border: none !important; box-shadow: none !important;">
<img src="/logos/epfl.png" alt="EPFL" style="max-width: 100%; max-height: 100%; object-fit: contain;">
</a>
<a href="https://ethz.ch/" target="_blank" style="display: flex; align-items: center; justify-content: center; width: 200px; height: 100px; text-decoration: none !important; border: none !important; box-shadow: none !important;">
<img src="/logos/eth-dark.png" alt="ETH Zürich" style="max-width: 100%; max-height: 100%; object-fit: contain;">
</a>
</div>