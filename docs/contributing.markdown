---
layout: default
title: Contributing
nav_order: 90
---

# Contributing to the SYNTH Initiative

## Current Contributors

The following people and organizations have contributed to the creation and maintenance of this project:

* [pleias](https://pleias.fr){:target="_blank"}
* [IBM](https://ibm.com){:target="_blank"}

<a name="join-this-project"></a>
## Join this Project Work Group

Want to help us drive the evolution of this project? Please join our work group. 

Use the form on the Alliance's [Become a collaborator](https://thealliance.ai/become-a-collaborator){:target="join-collab"} page to let us know your interests. 

In the &ldquo;Message&rdquo; box mention this project, **SYNTH Initiative**, and add anything else you would like us to know.

If your organization would like to join the AI Alliance, go [here](https://thealliance.ai/membership){:target="join-org"}.

## Other Ways to Contribute to this Project

### Contribute Your Dataset

Use this form to tell us about your dataset and where it is hosted. The form will open your email client with the information added and formatted. After we receive your email, we will follow up with next steps.

<div class="callout-box centered">
  <strong>For questions, send us email at <a href="mailto:data@thealliance.ai?subject=I%20have%20questions%20about%20contributing%20a%20SYNTH%20dataset">data@thealliance.ai</a>.</strong>
</div>
<form id="datasets-form">
    <!-- <div class="form-dataset disabled" inert> -->
    <div class="form-dataset"> 
        <table class="form-dataset-table">
            <tr>
                <th class="form-dataset-table-label">
                  <label for="dataset-name">Dataset&nbsp;name:</label>
                </th>
                <td class="form-dataset-table-value">
                  <input type="text" id="dataset-name" name="dataset-name" class="form-dataset-table-input" placeholder="A descriptive and unique name" required />   
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                  <label for="dataset-location">Dataset&nbsp;location:</label>
                </th>
                <td class="form-dataset-table-value">
                  <input type="url" id="dataset-url" name="dataset-url" class="form-dataset-table-input" placeholder="https://some-special-place.com" pattern="https://.*" required />
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                  <label for="dataset">Dataset&nbsp;card:</label>
                </th>
                <td class="form-dataset-table-value">
                  <input type="url" id="dataset-card" name="dataset-url" class="form-dataset-table-input" placeholder="https://some-special-place.com" pattern="https://.*" /> Leave blank if the dataset is hosted by Hugging Face and the README <em>is</em> the dataset card.
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                &nbsp;
                </th>
                <td class="form-dataset-table-value">
                  <input type="submit" value="Submit!" />
                </td>
            </tr>
        </table>
    </div>
</form>
<script>
  <!-- Necessary to have the file browser limit all the allowed sections to what "accept=''" specifies: -->
  var test = document.querySelector('input');

  const form = document.getElementById('datasets-form');
        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            const body1 = `body=dataset-name: ${document.getElementById('dataset-name').value}
dataset-url: ${document.getElementById('dataset-url').value}
dataset-card: ${document.getElementById('dataset-card').value}
            `;
            const body = body1.replace(/ /g, '%20').replace(/:/g, '%3A').replace(/\n/g, '%0D%0A');
            const mailto = `mailto:data@thealliance.ai?subject=I%20want%20to%20contribute%20a%20SYNTH%20dataset&${body}`
            try {
                window.open(mailto, '_contribute_email').focus();
            } catch (error) {
                console.error('Error formatting or submitting an email:', error);
            }
        });
</script>

### Post Issues, Discussions, Email, and Pull Requests

* Post a [discussion topic](https://github.com/The-AI-Alliance/SYNTH-initiative/discussions){:target="discussions"} 
* Post an [issue](https://github.com/The-AI-Alliance/SYNTH-initiative/issues){:target="issues"} 
* Send us [email](mailto:data@thealliance.ai?subject=The SYNTH project). This is a general email address, so be sure to mention this particular project.

[Pull requests](https://github.com/The-AI-Alliance/SYNTH-initiative/pulls){:target="pulls"} (PRs) are one way to contribute significant new content and other assets. For simple page edits, each website page has an _Edit this page on GitHub_ link for quick suggestions.

For bigger PR contributions, please see our [Alliance community repo](https://github.com/The-AI-Alliance/community/) for general information about contributing to any of our projects. This section provides some specific details you need to know.

In particular, see the AI Alliance [CONTRIBUTING](https://github.com/The-AI-Alliance/community/blob/main/CONTRIBUTING.md) instructions. You will need to agree with the AI Alliance [Code of Conduct](https://github.com/The-AI-Alliance/community/blob/main/CODE_OF_CONDUCT.md).

All _code_ contributions are licensed under the [Apache 2.0 LICENSE](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.Apache-2.0) (which is also in this repo, [LICENSE.Apache-2.0](LICENSE.Apache-2.0)).

All _documentation_ contributions are licensed under the [Creative Commons Attribution 4.0 International](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.CC-BY-4.0) (which is also in this repo, [LICENSE.CC-BY-4.0](LICENSE.CC-BY-4.0)).

All _data_ contributions are licensed under the [Community Data License Agreement - Permissive - Version 2.0](https://github.com/The-AI-Alliance/community/blob/main/LICENSE.CDLA-2.0) (which is also in this repo, [LICENSE.CDLA-2.0](LICENSE.CDLA-2.0)).

