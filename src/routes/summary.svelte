<script>
  import { onMount } from "svelte";

  onMount(() => {
    console.log("mounting v2...");
    window.GOVUKFrontend.initAll();
  });
</script>

<style>
</style>

<svelte:head>
  <title>gov.uk | sample summary</title>
</svelte:head>

<div class="govuk-breadcrumbs ">
  <ol class="govuk-breadcrumbs__list">
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Home</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Passports, travel and living abroad</a>
    </li>
    <li class="govuk-breadcrumbs__list-item">
      <a class="govuk-breadcrumbs__link" href="#">Travel abroad</a>
    </li>
  </ol>
</div>

<div class="govuk-!-padding-bottom-9">
<div class="govuk-panel govuk-panel--confirmation">
  <h1 class="govuk-panel__title">
    Application complete
  </h1>
  <div class="govuk-panel__body">
    Your reference number<br><strong>HDJ2123F</strong>
  </div>
</div>
<div class="govuk-phase-banner">
  <p class="govuk-phase-banner__content">
    <strong class="govuk-tag govuk-phase-banner__content__tag">
      alpha
    </strong>
    <span class="govuk-phase-banner__text">
      This is a new service – your <a class="govuk-link" href="#">feedback</a> will help us to improve it.
    </span>
  </p>
</div>
</div>

<dl class="govuk-summary-list">
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Name
    </dt>
    <dd class="govuk-summary-list__value">
      Sarah Philips
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> name</span>
      </a>
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Date of birth
    </dt>
    <dd class="govuk-summary-list__value">
      5 January 1978
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> date of birth</span>
      </a>
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Contact information
    </dt>
    <dd class="govuk-summary-list__value">
      72 Guild Street<br>London<br>SE23 6FH
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> contact information</span>
      </a>
    </dd>
  </div>
  <div class="govuk-summary-list__row">
    <dt class="govuk-summary-list__key">
      Contact details
    </dt>
    <dd class="govuk-summary-list__value">
      <p class="govuk-body">07700 900457</p>
      <p class="govuk-body">sarah.phillips@example.com</p>
    </dd>
    <dd class="govuk-summary-list__actions">
      <a class="govuk-link" href="#">
        Change<span class="govuk-visually-hidden"> contact details</span>
      </a>
    </dd>
  </div>
</dl>