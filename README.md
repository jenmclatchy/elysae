# Elysae

*A mirror for uncertain moments.*

Elysae is an iOS and web reflection app that pairs symbolic card selection with optional EEG self-observation and an AI-written reflection. You bring a question you cannot settle with more information; Elysae gives you a structured way to think it through, and shows you what your own brain activity did while you did.

**Try the web build:** [m897zdz94ywf9r1987sn.share.dreamflow.app](https://m897zdz94ywf9r1987sn.share.dreamflow.app/)

## The protocol

Each reflection follows the workflow set out in the accompanying capstone paper ([Structured Symbolic Reflection and Predictive Processing](https://github.com/jenmclatchy/structured-symbolic-reflection)):

1. **Question.** You write down what you are uncertain about.
2. **Baseline EEG.** A short resting recording (optional, with a Muse headband).
3. **Symbolic selection.** You draw a card, intuitively or by choosing an image.
4. **Reflection.** You sit with the card's meaning in relation to your question.
5. **Post-reflection EEG.** A second short recording.
6. **Comparison.** Baseline and post-reflection activity are compared.
7. **Reflective output.** An AI-generated interpretation that weaves together the card, your written reflection, and the change in your recordings.

The idea, from the paper: under unresolvable uncertainty, a symbolic system can act as an interpretive scaffold that lets affective signals be organised into a narrative, which updates the internal model and lowers subjective uncertainty even when nothing about the situation has changed.

## What is built

- Cross-platform app built in Dreamflow (Flutter), shipped through TestFlight and submitted to App Store Connect, with a shareable web build
- Firebase for Google and email sign-in and per-user Firestore storage of past reflections
- EEG biofeedback through a Muse headband and the Mind Monitor app
- AI reflections through an OpenAI configuration loaded at runtime from Firestore, so keys never ship in the client

## Status

Functional and in testing. The app has not been used to collect research data; any study would need ethics approval first.

## Source

The app is authored in Dreamflow, whose project files live in that platform rather than in a conventional source tree. This repository documents the design and links the live build. Exported Flutter source will be added here when it is pulled out of Dreamflow.
