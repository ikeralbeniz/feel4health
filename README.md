# FEEL 4 Health

**FEEL 4 Health** is a curated collection of practical examples, patterns, and “recipes” for using the **FEEL (Friendly Enough Expression Language)** syntax in **healthcare environments**. Its purpose is to support healthcare professionals, modelers, and analysts in creating accurate and maintainable **decision logic** within BPM+ ecosystems, including **DMN**, **BPMN**, and **CMMN**.

---

## 🩺 Purpose

BPM+ Health promotes the use of standards-based modeling to represent clinical pathways, decisions, and case management logic. However, expressing clinical rules with **FEEL** can be challenging for newcomers.

**FEEL 4 Health** aims to:

* Provide **realistic FEEL examples** designed specifically for clinical and administrative scenarios
* Clarify how to express **decision rules** in DMN using best practices
* Support healthcare professionals who need to model logic without deep programming knowledge
* Create a **community-driven reference library** of FEEL-based decision patterns

---

## 📁 Repository Structure

Each example or “recipe” follows a standardized template to ensure clarity and reusability:

### **1. Clinical Context**

A short description of the real-world healthcare scenario.
*Example: “A patient takes daily blood pressure measurements for one month.”*

### **2. Rule to Validate**

The logic expressed in natural language.
*Example: “Flag potential hypertension if more than 25% of systolic readings exceed 140 mmHg.”*

### **3. FEEL Expression**

A ready-to-use snippet implementing the rule.

```feel
count(bpReadings[ systolic > 140 ]) / count(bpReadings) > 0.25
```

---

## 💬 Community Discussion

The project encourages active participation and discussion to improve and refine the FEEL recipes. Users can:

* Propose improvements
* Submit alternative FEEL implementations
* Request clarifications
* Suggest new clinical scenarios

GitHub **Issues** and **Discussions** serve as the main channels for collaboration.

---

## 🧪 Playground Environment

To facilitate experimentation and learning, **FEEL 4 Health** will include a **playground environment** where users can:

* Test FEEL expressions interactively
* Modify recipes and try variations
* Validate rules with sample clinical data
* Share and discuss expression ideas

### **Playground Foundation**

The playground for this project is based on the open-source **feel-playground** developed by **@nikku**, available on GitHub:

[https://github.com/nikku/feel-playground](https://github.com/nikku/feel-playground)

This project will use and extend that environment to support healthcare-oriented examples and datasets.

---

## 🧠 Who Is This For?

* Healthcare professionals engaged in BPM+ modeling
* Clinical pathway and guideline modelers
* Decision support analysts
* Anyone learning FEEL in a healthcare-focused context

No programming background is necessary.

---

## 🧩 Topics Covered

Examples span common healthcare modeling needs, including:

* Vital signs and measurement interpretation
* Diagnostic and screening criteria
* Medication and dosage checks
* Administrative and eligibility rules
* Risk score calculations
* Temporal logic (follow-ups, intervals, recurrences)
* Clinical alerts and thresholds

All following the **context → rule → FEEL** pattern.

---

## 🤝 Contributions Welcome

This project is open and community-driven. Contributions are encouraged in the form of:

* New clinical scenarios and FEEL recipes
* Improvements to existing examples
* Feedback and discussion
* Enhancements to the playground environment

Pull requests, issues, and discussions are all welcome.

---

## 📜 License — **GNU AGPL-3.0**

FEEL 4 Health is released under the **GNU Affero General Public License v3.0 (AGPL-3.0)**.

This license ensures that:

* Any modified versions, including those deployed as services, must also be released under AGPL-3.0
* Improvements remain free and accessible to the community
* Contributions continue to support the openness of the ecosystem

The full license text is provided in the `LICENSE` file.
