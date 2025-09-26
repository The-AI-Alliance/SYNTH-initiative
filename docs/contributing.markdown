---
layout: default
title: Contributing
nav_order: 90
---

# Contributors

The following people and organizations have contributed to the creation and maintenance of this project:

* TODO

# How to Contribute to this Project

We welcome your contributions! 


## Contribute Your Dataset

Use this form to tell us about your dataset and where it is hosted. It will open your email client with the information added and formatted. After we receive your email, we will follow up with next steps.

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
            <!--
            <tr>
                <th class="form-dataset-table-label">
                  <label for="dataset-hosting">Hosting:</label>
                </th>
                <td class="form-dataset-table-value">
                  <input type="checkbox" id="dataset-alliance-hosting" name="dataset-alliance-hosting" unchecked /> I want the AI Alliance to host this dataset.
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                  <label for="modality">Modalities:</label>
                </th>
                <td class="form-dataset-table-value">
                    <div>
                      <input type="checkbox" id="dataset-modality-text" name="dataset-modality-text" class="form-dataset-table-checkbox" checked />
                      <label for="text">Text</label>
                    </div>
                    <div>
                      <input type="checkbox" id="dataset-modality-text" name="dataset-modality-text" class="form-dataset-table-checkbox" />
                      <label for="images">Images</label>
                    </div>
                    <div>
                      <input type="checkbox" id="dataset-modality-text" name="dataset-modality-text" class="form-dataset-table-checkbox" />
                      <label for="audio">Audio</label>
                    </div>
                    <div>
                      <input type="checkbox" id="dataset-modality-text" name="dataset-modality-text" class="form-dataset-table-checkbox" />
                      <label for="video">Video (including audio)</label>
                    </div>
                    <div>
                      <input type="checkbox" id="dataset-modality-text" name="dataset-modality-text" class="form-dataset-table-checkbox" />
                      <label for="video">Other (e.g., science data)</label>
                    </div>
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                    <label for="domain">Domain:</label>
                </th>
                <td class="form-dataset-table-value">
                  <select id="dataset-domain" name="dataset-domain" class="form-dataset-table-input">
                    <optgroup label="General Purpose">
                      <option default>Not domain specific</option>
                    </optgroup>
                    <optgroup label="Science & Industrial">
                      <option>Climate</option>
                      <option>Marine</option>
                      <option>Materials</option>
                      <option>Semiconductors</option>
                      <option>Time Series</option>
                      <option>Other Industrial</option>
                    </optgroup>
                    <optgroup label="Other">
                      <option>Finance</option>
                      <option>Healthcare</option>
                      <option>Legal</option>
                      <option>Social Science</option>
                    </optgroup>
                  </select>
                  Or another domain? 
                  <input type="text" id="dataset-other-domain" name="dataset-other-domain" class="form-dataset-table-input-shorter" placeholder="Your domain suggestion" required />
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                  <label for="email">Email:</label>
                </th>
                <td class="form-dataset-table-value">
                  <input type="email" id="email" name="email" class="form-dataset-table-input" placeholder="Your email address" required />   
                </td>
            </tr>
            <tr>
                <th class="form-dataset-table-label">
                &nbsp;
                </th>
                <td class="form-dataset-table-value">
                  <input type="checkbox" id="agree-to-terms" name="agree-to-terms" required /> I agree to the terms for contribution.
                </td>
            </tr>
            -->
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
            const body = body1.replace(/ /g, '%20').replace(/:/g, '%3A%20').replace(/\n/g, '%0D%0A');
            const mailto = `mailto:data@thealliance.ai?subject=I%20want%20to%20contribute%20a%20SYNTH%20dataset&${body}`
            try {
                window.open(mailto, '_contribute_email').focus();
            } catch (error) {
                console.error('Error formatting or submitting an email:', error);
            }
        });
</script>

## Other Ways to Contribute

Ways to suggest ideas:
* Post a [discussion topic](https://github.com/The-AI-Alliance/SYNTH-initiative/discussions){:target="discussions"} 
* Post an [issue](https://github.com/The-AI-Alliance/SYNTH-initiative/issues){:target="issues"} 
* Send us [email](mailto:data@thealliance.ai). This is a general email address, so be sure to mention this particular project.

Want to offer new content?
* Post a [pull request](https://github.com/The-AI-Alliance/SYNTH-initiative/pulls){:target="prs"}! 
	* For corrections to existing pages, note that every page has an _Edit this page on GitHub_ link, which goes straight to the page's source. Make your edits there and submit a PR! This is the best way to help us fix typos and make other small improvements.

For general information about contributing to AI Alliance projects, visit [this `community` repo](https://github.com/The-AI-Alliance/community/){:target="community"}, specifically the [`CONTRIBUTING` page](https://github.com/The-AI-Alliance/community/blob/main/CONTRIBUTING.md){:target="community"} for general information about contributing. 

See also the full list of projects [here](https://the-ai-alliance.github.io/){:target="aia-github"} to find other projects that might interest you.

{% comment %}
Keep the following anchor in case you change the section "Join..." text. 
The link is used by the default docs/_includes/header_buttons_custom.html, for example.
{% endcomment %}
<a name="join-this-project"></a>
## Join this Project Work Group

Want to help us drive the evolution of this project? Please join our work group. 

Use the form on the Alliance's [Become a collaborator](https://thealliance.ai/become-a-collaborator){:target="join-collab"} page to let us know your interests. 

In the &ldquo;Message&rdquo; box mention this project, **SYNTH Initiative**, and add anything else you would like us to know.

If your organization would like to join the AI Alliance, go [here](https://thealliance.ai/membership){:target="join-org"}.

## Other Notes on Contributing

The sources for this website are in the GitHub repo's [`docs`](https://github.com/The-AI-Alliance/SYNTH-initiative/tree/main/docs){:target="repo-docs"} directory. 

Notice that every page on this website has an _Edit this page on GitHub_ link to the corresponding location for the page in the GitHub repo, making it easy to view a page, then go straight to the source, make edits, and submit a PR! This is the best way to help us fix typos and make other small improvements.

This documentation is built with [GitHub Pages](https://pages.github.com/){:target="github-pages"}, which uses [Jekyll](https://github.com/jekyll/jekyll){:target="gh-jekyll"} to serve the website. We use the [Just the Docs](https://just-the-docs.github.io/just-the-docs/){:target="just-the-docs"} Jekyll theme. See the repo file [`GITHUB_PAGES.md`](https://github.com/The-AI-Alliance/SYNTH-initiative/tree/main/GITHUB_PAGES.md){:target="_blank"} for more information.
