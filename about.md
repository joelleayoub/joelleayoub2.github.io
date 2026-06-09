---
layout: default
title: About
permalink: /about/
---

<div class="hero-section" style="padding: 100px 0; background: var(--background-color); border-bottom: 1px solid var(--border-color); text-align: center;">
    <div class="container">
        <h1 style="font-size: var(--font-size-3xl); letter-spacing: -0.02em; color: var(--text-primary);">About Joelle Ayoub</h1>
        <p style="color: var(--text-secondary); opacity: 0.9; max-width: 800px; margin: 0 auto; font-weight: 300;">I am a robotics and mechatronics engineer focused on building reliable embedded systems, mechanical designs, and interactive visualizations. This site showcases my projects, designs, and code.</p>
    </div>
</div>

<div class="about-content">
    <div class="container">
        <section class="about-section">
            <h2>About Me</h2>
            <p>Hi — I'm Joelle Ayoub. I work at the intersection of mechanical design, electronics, and software. I enjoy turning ideas into working prototypes, from PCBs and firmware to 3D models and web visualizations.</p>
            <p>My interests include embedded systems, ROS, control systems, sensors, and rapid prototyping. I document projects here with schematics, model previews, and the code used to build them.</p>
        </section>

        <section class="about-section">
            <h2>Skills & Tools</h2>
            <ul>
                <li>Embedded C/C++, Python, Robot Operating System (ROS)</li>
                <li>PCB design (KiCad), sensor integration, and electronics debugging</li>
                <li>3D CAD and model preparation for printing and visualization</li>
                <li>Web visualizations, Jekyll, and GitHub Pages</li>
            </ul>
        </section>

        <section class="about-section">
            <h2>Get in Touch</h2>
            <p>You can find my work on <a href="https://github.com/{{ site.github_username }}" target="_blank">GitHub</a> or contact me at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.</p>
        </section>
    </div>
</div>

<style>
/* Keep styles minimal and rely on existing site styles */
.about-content { padding: var(--spacing-2xl) 0; }
.about-section { margin-bottom: var(--spacing-3xl); }
.about-section h2 { color: var(--text-primary); margin-bottom: var(--spacing-md); }
</style>
}

.about-section {
    margin-bottom: var(--spacing-3xl);
}

.about-section h2 {
    color: var(--text-primary);
    margin-bottom: var(--spacing-lg);
    padding-bottom: var(--spacing-sm);
    border-bottom: 1px solid var(--border-color);
    font-size: var(--font-size-2xl);
    letter-spacing: -0.01em;
}

.features-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: var(--spacing-xl);
    margin-top: var(--spacing-lg);
}

.feature-item {
    padding: var(--spacing-lg);
    background-color: var(--surface-color);
    border-radius: var(--radius-sm);
    border: none;
    box-shadow: 0 4px 20px var(--shadow-color);
    transition: transform var(--transition-normal), box-shadow var(--transition-normal);
}

.feature-item:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 30px var(--shadow-hover);
}

.feature-item h3 {
    display: flex;
    align-items: center;
    gap: var(--spacing-sm);
    color: var(--text-primary);
    margin-bottom: var(--spacing-md);
}

.feature-item h3 i {
    color: var(--primary-color);
    font-size: var(--font-size-lg);
}

.perfect-for-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--spacing-lg);
    margin-top: var(--spacing-lg);
}

.perfect-for-item {
    text-align: center;
    padding: var(--spacing-lg);
    background-color: var(--surface-color);
    border-radius: var(--radius-lg);
    border: 1px solid var(--border-color);
}

.perfect-for-item h4 {
    color: var(--primary-color);
    margin-bottom: var(--spacing-sm);
}

.tech-stack {
    display: flex;
    flex-wrap: wrap;
    gap: var(--spacing-lg);
    justify-content: center;
    margin-top: var(--spacing-lg);
}

.tech-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: var(--spacing-sm);
    padding: var(--spacing-lg);
    background-color: var(--surface-color);
    border-radius: var(--radius-lg);
    border: 1px solid var(--border-color);
    min-width: 120px;
}

.tech-item i {
    font-size: var(--font-size-2xl);
    color: var(--accent-color);
}

.tech-item span {
    font-weight: var(--font-weight-medium);
    color: var(--text-primary);
}

.getting-started-steps {
    background-color: var(--surface-color);
    padding: var(--spacing-xl);
    border-radius: var(--radius-lg);
    border: 1px solid var(--border-color);
    margin: var(--spacing-lg) 0;
}

.getting-started-steps li {
    margin-bottom: var(--spacing-md);
    line-height: var(--line-height-relaxed);
}

.cta-buttons {
    display: flex;
    gap: var(--spacing-md);
    justify-content: center;
    flex-wrap: wrap;
    margin-top: var(--spacing-xl);
}

@media (max-width: 640px) {
    .features-list {
        grid-template-columns: 1fr;
    }
    
    .perfect-for-grid {
        grid-template-columns: 1fr;
    }
    
    .tech-stack {
        justify-content: center;
    }
    
    .cta-buttons {
        flex-direction: column;
        align-items: center;
    }
}
</style>