# Architecture

## Overview

Market Research Engine is a pipeline that turns a raw idea into a sourced market report.

## Components

- Idea Intake: accepts a plain-text idea and asks clarifying questions when needed.
- Classifier: maps the idea to markets, segments, keywords, and competitor categories.
- Source Collector: gathers public pages, reviews, trend signals, directories, and marketplace data.
- Extractor: extracts competitors, pricing, claims, pains, audiences, and feature patterns.
- Evidence Store: stores source URL, date, excerpt, and derived claims.
- Analyzer: groups findings and separates facts from estimates.
- Report Generator: creates the final report with summary, risks, opportunities, and next experiments.

## Data Flow

1. User submits an idea.
2. The classifier creates search targets.
3. The collector gathers public sources.
4. The extractor turns sources into structured facts.
5. The analyzer finds patterns and gaps.
6. The generator writes a report with source links.

## Key Design Rule

Every important claim should point back to a source or be clearly marked as an estimate.

## MVP Architecture

The MVP can start as a semi-automated workflow: automated structure, manual review of sources, and generated reports.
