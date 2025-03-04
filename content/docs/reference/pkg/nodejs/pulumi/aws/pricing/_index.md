---
title: "Module pricing"
linktitle: "pricing"
meta_desc: "Explore members of the pricing module in the @pulumi/aws package."
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-aws` repo](https://github.com/pulumi/pulumi-aws/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-aws` repo](https://github.com/terraform-providers/terraform-provider-aws/issues).






<h3>Data Sources</h3>
<ul class="api">
    <li><a href="#getProduct"><span class="symbol datasource"></span>getProduct</a></li>
</ul>

<h3>Others</h3>
<ul class="api">
    <li><a href="#GetProductArgs"><span class="symbol api"></span>GetProductArgs</a></li>
    <li><a href="#GetProductResult"><span class="symbol api"></span>GetProductResult</a></li>
</ul>



<h2 id="data-sources">Data Sources</h2>
<h3 class="pdoc-module-header" id="getProduct" data-link-title="getProduct">
    <a href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L71">
        Data Source <strong>getProduct</strong>
    </a>
</h3>


<pre class="highlight"><code><span class='kd'></span>getProduct(args: <a href='#GetProductArgs'>GetProductArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions'>pulumi.InvokeOptions</a>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#GetProductResult'>GetProductResult</a>&gt; &amp; <a href='#GetProductResult'>GetProductResult</a></code></pre>


Use this data source to get the pricing information of all products in AWS.
This data source is only available in a us-east-1 or ap-south-1 provider.

#### Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const example = aws.pricing.getProduct({
    filters: [
        {
            field: "instanceType",
            value: "c5.xlarge",
        },
        {
            field: "operatingSystem",
            value: "Linux",
        },
        {
            field: "location",
            value: "US East (N. Virginia)",
        },
        {
            field: "preInstalledSw",
            value: "NA",
        },
        {
            field: "licenseModel",
            value: "No License required",
        },
        {
            field: "tenancy",
            value: "Shared",
        },
    ],
    serviceCode: "AmazonEC2",
});
```

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const example = aws.pricing.getProduct({
    filters: [
        {
            field: "instanceType",
            value: "ds1.xlarge",
        },
        {
            field: "location",
            value: "US East (N. Virginia)",
        },
    ],
    serviceCode: "AmazonRedshift",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/d/pricing_product.html.markdown.


<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="GetProductArgs" data-link-title="GetProductArgs">
    <a href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L90">
        interface <strong>GetProductArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetProductArgs</span></code></pre>

A collection of arguments for invoking getProduct.

<h4 class="pdoc-member-header" id="GetProductArgs-filters">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L94">property <b>filters</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>filters: <a href='/docs/reference/pkg/nodejs/pulumi/aws/types/input/#GetProductFilter'>inputs.pricing.GetProductFilter</a>[];</code></pre>

A list of filters. Passed directly to the API (see GetProducts API reference). These filters must describe a single product, this resource will fail if more than one product is returned by the API.

<h4 class="pdoc-member-header" id="GetProductArgs-serviceCode">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L98">property <b>serviceCode</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>serviceCode: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The code of the service. Available service codes can be fetched using the DescribeServices pricing API call.

<h3 class="pdoc-module-header" id="GetProductResult" data-link-title="GetProductResult">
    <a href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L104">
        interface <strong>GetProductResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetProductResult</span></code></pre>

A collection of values returned by getProduct.

<h4 class="pdoc-member-header" id="GetProductResult-filters">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L105">property <b>filters</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>filters: <a href='/docs/reference/pkg/nodejs/pulumi/aws/types/output/#GetProductFilter'>outputs.pricing.GetProductFilter</a>[];</code></pre>
<h4 class="pdoc-member-header" id="GetProductResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L114">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

id is the provider-assigned unique ID for this managed resource.

<h4 class="pdoc-member-header" id="GetProductResult-result">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L109">property <b>result</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>result: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

Set to the product returned from the API.

<h4 class="pdoc-member-header" id="GetProductResult-serviceCode">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/f1cda9e4c1dc7d1df742e78fa5956d1fae9f9e65/sdk/nodejs/pricing/getProduct.ts#L110">property <b>serviceCode</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>serviceCode: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>
