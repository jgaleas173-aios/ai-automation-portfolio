# AI OS Control Center

[Back to portfolio](../README.md)

**Project visibility without turning the dashboard into an execution authority.**

## Problem

AI-assisted projects can accumulate status across handoffs, task records, and evidence files. A useful dashboard should make that information understandable without interpreting a status update as permission to change the project.

## Approach

The project documents a local Windows control center that reads project evidence and presents status separately from the execution path. Its stated safety boundary excludes repair-script execution, gate approval, and changes to project permissions.

The documented design keeps unavailable or uncertain evidence conservative rather than modifying the source to make the dashboard appear healthy.

## Repository evidence

*Evidence snapshot: October 8, 2026.*

The repository includes Python components, PowerShell support scripts, and web assets. Its GitHub Actions workflow checks for tracked generated state, compiles Python source, parses PowerShell source, checks required documentation markers, and verifies that required web assets exist.

At the October 8, 2026 inspection, the recorded main-branch run from October 7, 2026 had completed successfully. These are static and repository-level checks; the portfolio review did not reproduce the live dashboard, polling behavior, watcher reliability, or end-to-end safety properties.

## My contribution

I focus on defining what the status surface should communicate, keeping observation separate from authority, and making missing evidence visible rather than treating it as a successful state.

## Important tradeoff

A dashboard that cannot execute corrective actions is less convenient than a one-click control panel, but it has a narrower operational role. The distinction makes the safety boundary easier to describe and review.

## Status and limitations

A private local operational tool with machine-specific configuration. The existing README is an operator guide, not a portable public installation guide. A public demonstration would need synthetic project data and a separate review of the demonstrated build.

No screenshot of private project status or source evidence is included in this case study.
