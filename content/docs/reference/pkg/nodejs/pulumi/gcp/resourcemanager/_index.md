---
title: Module resourcemanager
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/gcp</a> &gt; resourcemanager

<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Lien">class Lien</a></li>
<li><a href="#LienArgs">interface LienArgs</a></li>
<li><a href="#LienState">interface LienState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts">resourcemanager/lien.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Lien">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L30">class <b>Lien</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

A Lien represents an encumbrance on the actions that can be performed on a resource.

## Example Usage - Resource Manager Lien


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const project = new gcp.organizations.Project("project", {
    projectId: "staging-project",
});
const lien = new gcp.resourcemanager.Lien("lien", {
    origin: "machine-readable-explanation",
    parent: pulumi.interpolate`projects/${project.number}`,
    reason: "This project is an important environment",
    restrictions: ["resourcemanager.projects.delete"],
});
```

{{% /md %}}
<h3 class="pdoc-member-header" id="Lien-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L48"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Lien(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#LienArgs'>LienArgs</a>, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Lien resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L39">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#LienState'>LienState</a>, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Lien'>Lien</a></pre>


Get an existing Lien resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L143">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L43">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>createTime: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L138">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L44">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-origin">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L45">property <b>origin</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>origin: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-parent">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L46">property <b>parent</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>parent: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-reason">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L47">property <b>reason</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>reason: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-restrictions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L48">property <b>restrictions</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>restrictions: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Lien-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="LienArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L115">interface <b>LienArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Lien resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="LienArgs-origin">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L116">property <b>origin</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>origin: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienArgs-parent">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L117">property <b>parent</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>parent: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienArgs-reason">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L118">property <b>reason</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>reason: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienArgs-restrictions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L119">property <b>restrictions</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>restrictions: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="LienState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L103">interface <b>LienState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Lien resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="LienState-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L104">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>createTime?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L105">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienState-origin">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L106">property <b>origin</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>origin?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienState-parent">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L107">property <b>parent</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>parent?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienState-reason">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L108">property <b>reason</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>reason?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LienState-restrictions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/092a9ff4cb31b7c591f6b8a6df2fc79275ad6d36/sdk/nodejs/resourcemanager/lien.ts#L109">property <b>restrictions</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>restrictions?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>