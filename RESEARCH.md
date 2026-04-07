# Neurodivergent Design Research

This document records the evidence-based rationale behind every design decision in the Focus Timer. The timer was built for a 9-year-old with ADHD and a 12-year-old with high-functioning autism. Each choice below is grounded in peer-reviewed research or published clinical guidance.

---

## 1. Transition Warnings (Last-5-Seconds Countdown)

**Design decision:** At 5 seconds remaining, the display switches from MM:SS to a large single-digit countdown (5, 4, 3, 2, 1) in amber, with a gentle pulse each second.

**Why:**
Autistic individuals have significantly greater difficulty shifting attention from one task to another, often due to a strong need for predictability and challenges in understanding what activity comes next. Explicit, advance visual warnings substantially reduce transition-related meltdowns and improve cooperative behavior. Research from the Indiana Resource Center for Autism documents that children with autism who receive structured time warnings show reduced transition time, increased appropriate behavior, and decreased reliance on adult prompting.

Occupational therapists routinely set visual timers at 2–5 minutes remaining as preparation cues, precisely because the transition itself — not the ending — is the source of distress.

**References:**
- Indiana Resource Center for Autism. *Transition Time: Helping Individuals on the Autism Spectrum Move Successfully from One Activity to Another.* https://iidc.indiana.edu/irca/articles/transition-time-helping-individuals-on-the-autism-spectrum-move-successfully-from-one-activity-to-another.html
- Leaf Wing Center. *Using Time Warnings To Help Students With Autism.* https://leafwingcenter.org/using-time-warnings-to-help-students-with-autism/
- Time Timer. *Occupational Therapy Tools for Time Management.* https://www.timetimer.com/blogs/news/occupational-therapy-tools-for-time-management

---

## 2. Calm Animation Over Urgency (Scale 1.04, Not Aggressive Zoom)

**Design decision:** The last-5-seconds pulse scales the digit to 1.04× (barely perceptible growth), not the large zoom-in/zoom-out seen in physical therapy apps designed for adults.

**Why:**
An eye-tracking study by Hanley, Fox, and Khairat (2018) found that autistic users are significantly more distracted and frustrated by animation than neurotypical users — motion serves as a constant point of distraction because the eye is attracted to movement even when attention is directed elsewhere. Autistic participants in the study required substantially greater mental effort to complete tasks in the presence of animated elements.

Dr. Emily King, a child psychologist specializing in ADHD and autism, documents that visual countdown urgency (aggressive animations, escalating alarms) increases anxiety rather than reducing it: "When we experience high anxiety we cannot learn or complete the task in front of us." The opposite of anxiety is trust, built through calm and predictable design.

Large-scale zoom animations also approach the threshold for visual overstimulation. Up to 70% of autistic individuals experience atypical visual processing, and content that flashes or rapidly changes scale is a known sensory trigger.

**References:**
- Hanley, M., Fox, J., & Khairat, M. (2018). *Classroom Displays — Attraction or Distraction? Evidence of Impact on Attention and Learning From Children With and Without Autism.* Developmental Psychology. https://pubmed.ncbi.nlm.nih.gov/28471220/
- King, E. W., Ph.D. *But Timers Make My Kid Anxious.* Learn with Dr. Emily. https://learnwithdremily.substack.com/p/but-timers-make-my-kid-anxious
- TheraSpecs. *Light Sensitivity and Autism Spectrum Disorder.* https://www.theraspecs.com/blog/light-sensitivity-autism/

---

## 3. Ding Spacing (3 Seconds Between Dings)

**Design decision:** Alert dings are spaced 3 seconds apart instead of 1 second. A soft warning ding fires at the 3-second mark before the timer ends.

**Why:**
Research on auditory processing in autism supports longer intervals between acoustic events. A 1-second gap is too short for full auditory processing — the brain has not finished analyzing the first sound before the second arrives, which can cause auditory overload. A 3-second interval allows complete processing of each tone and acts as a distinct, interpretable attention cue rather than a barrage.

For ADHD, distinct timed sounds serve as working-memory anchors — a well-spaced sequence of tones ("three dings = timer done") is easier to internalize as a predictable signal than a rapid burst. ADHD coaching literature recommends multiple spaced alarms (e.g., a 30-minute warning, 10-minute warning, and final alarm) precisely because spaced, distinct cues are more effective than a single jarring alert.

**References:**
- Take Control ADHD. *Sound the Alarm.* https://takecontroladhd.com/blog/sound-the-alarm
- Tiimo App. *Sensory-Friendly Design for ADHD and Autism Planning.* https://www.tiimoapp.com/resource-hub/sensory-design-neurodivergent-accessibility

---

## 4. Mute Toggle

**Design decision:** A mute button is always visible and persists its state. When muted, zero sound plays — including the end-of-phase chime and the 3-second warning ding.

**Why:**
Auditory hypersensitivity affects approximately 70% of autistic individuals. Unexpected or loud sounds — even gentle chimes — can be experienced as physically painful or acutely distressing. Timers with audible alerts are a documented source of anxiety: Dr. King reports children "putting their hands over their ears at the sight of a timer," anticipating the alarm sound.

Best practice in occupational therapy and autism education is to introduce timers in silent mode first to build positive associations, then gradually introduce sound if the child tolerates it. The mute toggle supports this approach by giving caregivers and children full control.

**References:**
- King, E. W., Ph.D. *But Timers Make My Kid Anxious.* https://learnwithdremily.substack.com/p/but-timers-make-my-kid-anxious
- TheraSpecs. *Light Sensitivity and Autism Spectrum Disorder.* https://www.theraspecs.com/blog/light-sensitivity-autism/
- Time Timer. *ADHD Timer.* https://www.timetimer.com/pages/adhd

---

## 5. Rounds / Defined Endpoint

**Design decision:** Users can select 1, 2, or 5 rounds. When a limit is set, the timer stops automatically after the final break with a celebratory message. Without a selection, the timer loops indefinitely.

**Why:**
A core need in autism is predictability — knowing exactly what will happen and when it will end. Open-ended tasks ("this could go on forever") are a documented source of anxiety for autistic children. Providing a concrete endpoint ("3 rounds, then we're done") gives the child a clear mental model of the session, reducing the cognitive load of wondering when to expect freedom.

For ADHD, defined goals with visible progress (round counter showing "Round 2 of 3") activate reward circuitry more effectively than open-ended tasks. Progress visibility is a key motivational scaffold in ADHD research.

**References:**
- Leaf Wing Center. *Transition Strategies for Autistic Students.* https://leafwingcenter.org/transition-strategies-autistic-students/
- Indiana Resource Center for Autism. *Transition Time.* https://iidc.indiana.edu/irca/articles/transition-time-helping-individuals-on-the-autism-spectrum-move-successfully-from-one-activity-to-another.html

---

## 6. Color Choices

**Design decision:** Focus phase uses an indigo gradient; break phase uses a teal gradient; the last-5-seconds warning uses amber (#f57c00). No red is used anywhere. Dark mode is automatically applied via `prefers-color-scheme`.

**Why:**
Autistic individuals frequently report that overly colorful or high-contrast environments are distracting and overwhelming, with preferences for muted, calming palettes and more white/neutral space. Indigo and teal are cool, low-saturation tones associated with calm and focus in color psychology, and are used in occupational therapy and autism classroom design.

Amber is used for the countdown warning (rather than red) because red carries universal alarm/danger associations that can trigger stress responses. Amber signals "attention / getting close" without the negative emotional loading of red. This aligns with traffic-light frameworks used in autism education (green = safe, yellow/amber = prepare, red = stop/danger) — we want "prepare", not "danger".

**References:**
- Tiimo App. *Sensory-Friendly Design for ADHD and Autism Planning.* https://www.tiimoapp.com/resource-hub/sensory-design-neurodivergent-accessibility
- Beacon School Support. *ASD Sensory Overload.* https://beaconschoolsupport.co.uk/newsletters/asd-sensory-overload-videos

---

## 7. Transition Messages (Positive Reinforcement Language)

**Design decision:** When a phase ends, the timer circle displays an encouraging message ("You did it! Time to rest." / "Recharged! Time to focus.") for 30 seconds before the next phase begins.

**Why:**
Social stories — short, predictable narrative phrases describing what is happening and what comes next — are an evidence-based intervention for autistic children (developed by Carol Gray, 1991). The transition messages follow this structure: they name the completed event, validate the effort, and describe what comes next in concrete terms.

The language uses autonomy-supportive phrasing drawn from self-determination theory (Deci & Ryan): phrases like "You earned a break" and "You got this!" validate the child's competence and autonomy rather than issuing directives. This framing is shown to increase intrinsic motivation and reduce resistance in neurodivergent learners.

The 30-second display time allows children who process language more slowly to read and internalize the message without feeling rushed into the next phase.

**References:**
- Gray, C. (1991). *Social Stories.* The Gray Center. https://carolgraysocialstories.com/
- Deci, E. L., & Ryan, R. M. *Self-Determination Theory.* https://selfdeterminationtheory.org/
- Leaf Wing Center. *Transition Strategies for Autistic Students.* https://leafwingcenter.org/transition-strategies-autistic-students/

---

## 8. Reduced-Motion Support

**Design decision:** The `@media (prefers-reduced-motion: reduce)` query disables all scale animations (ring pulse, countdown pulse) while preserving color changes and progress ring movement.

**Why:**
WCAG 2.1 Success Criterion 2.3.3 (AAA) requires that motion triggered by interaction can be disabled. Beyond compliance, this setting is commonly enabled by users with vestibular disorders, epilepsy, and visual hypersensitivity — all of which overlap significantly with the autism population. Motion on screen, even subtle animations, can cause nausea, disorientation, or cognitive overload in sensitive users.

The color change in the countdown (digits turning amber) is preserved even when motion is disabled because color alone conveys the warning without requiring any animation. This maintains the transition cue's usefulness for non-motion users.

**References:**
- W3C. *WCAG 2.1 — Success Criterion 2.3.3: Animation from Interactions.* https://www.w3.org/WAI/WCAG21/Understanding/animation-from-interactions.html
- IBM Accessibility. *Visual Design — Flashing and Motion.* https://www.ibm.com/able/toolkit/design/visual/flashing-and-motion/

---

## 9. Half-Volume Warning Ding

**Design decision:** The 3-second pre-end warning ding plays at half the volume of the end-of-phase chime (gain 0.08 vs 0.18).

**Why:**
Sudden, loud sounds are a primary distress trigger for autistic children with auditory hypersensitivity. A warning sound that is itself startling defeats its purpose — it creates the very anxiety it is meant to prevent. By making the warning softer than the end-of-phase chime, a clear acoustic hierarchy is established: soft ding = "almost there", louder chime sequence = "done". This layered, predictable structure supports the trust-building approach Dr. King recommends.

The warning ding uses the same C5/E5 tone pair as the end-of-phase chime so the child learns to associate that sound with a positive, familiar event (transition to rest or play), not with alarm.

**References:**
- King, E. W., Ph.D. *But Timers Make My Kid Anxious.* https://learnwithdremily.substack.com/p/but-timers-make-my-kid-anxious
- Time Timer. *ADHD Timer.* https://www.timetimer.com/pages/adhd
- Tiimo App. *Sensory-Friendly Design for ADHD and Autism Planning.* https://www.tiimoapp.com/resource-hub/sensory-design-neurodivergent-accessibility
