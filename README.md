Hi


I am currently pursuing my PhD at University of Texas at Austin. I'm passionate about exploring innovative solutions in energy engineering and contributing to the advancement of sustainable energy technologies.


Research Interests

    Energy Engineering
    Reservoir Characterization
    Modeling and Simulation
    Sustainable Energy Solutions
    Artificial Intelligence

Academic Research

    PhD Research: High-performance computing in subsurface hydrogen storage and generation
    MS Research: Impact of aperture distribution models on permeability estimation of outcrop-based fracture trace maps
    BE Research: Stress analysis of completion string in ultra-deep and high pressure gas wells
    

Skills and Tools

    Python, C++, C, Julia, Dataiku, Petrel, CMG, Data Analytics, MS Office Specialist, ArcGIS, ECLIPSE, Tableau, HFM, Machine Learning, Deep Learning.

const username = "s-tirmizi"; // Replace with your GitHub username

async function fetchLanguages() {
    const response = await fetch(`https://api.github.com/users/${username}/repos`);
    const repos = await response.json();
    let languageCount = {};

    for (const repo of repos) {
        if (repo.language) {
            languageCount[repo.language] = (languageCount[repo.language] || 0) + 1;
        }
    }

    return languageCount;
}

async function renderChart() {
    const languageData = await fetchLanguages();
    const ctx = document.getElementById("languageChart").getContext("2d");
    new Chart(ctx, {
        type: "bar",
        data: {
            labels: Object.keys(languageData),
            datasets: [{
                label: "Repositories per Language",
                data: Object.values(languageData),
                backgroundColor: "rgba(75, 192, 192, 0.5)",
                borderColor: "rgba(75, 192, 192, 1)",
                borderWidth: 1
            }]
        },
        options: {
            responsive: true,
            scales: {
                y: {
                    beginAtZero: true
                }
            }
        }
    });
}

document.addEventListener("DOMContentLoaded", renderChart);


Let's Connect!
    
<div style="padding-left: 10px;">
  📫 Email: stirmizi@utexas.edu<br>
  💼 LinkedIn: <a href="https://www.linkedin.com/in/talha-tirmizi/">Talha Tirmizi</a>
</div>
