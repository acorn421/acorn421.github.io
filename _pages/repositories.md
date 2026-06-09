---
layout: page
permalink: /repositories/
title: Repositories
description: A selection of open-source projects I contribute to.
nav: true
nav_order: 4
---

<style>
  .repo-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 1rem;
    margin-top: 1.5rem;
  }
  .repo-card {
    display: flex;
    flex-direction: column;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    padding: 1rem 1.1rem;
    background-color: var(--global-card-bg-color);
    transition: border-color 0.2s ease-in-out, transform 0.2s ease-in-out;
  }
  .repo-card:hover {
    border-color: var(--global-theme-color);
    transform: translateY(-2px);
  }
  .repo-card .repo-name {
    font-weight: 700;
    font-size: 1.05rem;
    color: var(--global-theme-color);
    word-break: break-word;
  }
  .repo-card .repo-owner {
    color: var(--global-text-color-light);
    font-weight: 400;
  }
  .repo-card .repo-desc {
    margin: 0.5rem 0 0.9rem;
    font-size: 0.92rem;
    color: var(--global-text-color);
    flex: 1 1 auto;
  }
  .repo-card .repo-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    font-size: 0.85rem;
    color: var(--global-text-color-light);
  }
  .repo-card .repo-meta .dot {
    display: inline-block;
    width: 0.7rem;
    height: 0.7rem;
    border-radius: 50%;
    margin-right: 0.35rem;
    vertical-align: middle;
  }
  @media (max-width: 576px) {
    .repo-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="repo-grid">
  <a class="repo-card" href="https://github.com/ossf/oss-crs" target="_blank" rel="noopener">
    <span class="repo-name"><span class="repo-owner">sslab-gatech / </span>OSS-CRS</span>
    <span class="repo-desc">Cyber Reasoning Systems for Bug-Finding and Patching in Open Source Software. I am a main contributor.</span>
    <span class="repo-meta">
      <span><span class="dot" style="background-color:#3572A5"></span>Python</span>
      <span>★ 90</span>
    </span>
  </a>

  <a class="repo-card" href="https://github.com/sslab-gatech/CRSBench" target="_blank" rel="noopener">
    <span class="repo-name"><span class="repo-owner">sslab-gatech / </span>CRSBench</span>
    <span class="repo-desc">Cyber Reasoning System Benchmark Suite for realistic end-to-end evaluation of CRS capabilities.</span>
    <span class="repo-meta">
      <span><span class="dot" style="background-color:#3572A5"></span>Python</span>
      <span>★ 5</span>
    </span>
  </a>
</div>
