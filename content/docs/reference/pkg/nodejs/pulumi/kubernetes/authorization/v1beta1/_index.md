---
title: Module authorization/v1beta1
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../../">@pulumi/kubernetes</a> &gt; <a href="../">authorization</a> &gt; v1beta1

<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#LocalSubjectAccessReview">class LocalSubjectAccessReview</a></li>
<li><a href="#SelfSubjectAccessReview">class SelfSubjectAccessReview</a></li>
<li><a href="#SelfSubjectRulesReview">class SelfSubjectRulesReview</a></li>
<li><a href="#SubjectAccessReview">class SubjectAccessReview</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts">authorization/v1beta1/LocalSubjectAccessReview.ts</a> <a href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts">authorization/v1beta1/SelfSubjectAccessReview.ts</a> <a href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts">authorization/v1beta1/SelfSubjectRulesReview.ts</a> <a href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts">authorization/v1beta1/SubjectAccessReview.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="LocalSubjectAccessReview">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L14">class <b>LocalSubjectAccessReview</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

LocalSubjectAccessReview checks whether or not a user or group can perform an action in a
given namespace. Having a namespace scoped resource makes it much easier to grant namespace
scoped policy that includes permissions checking.

{{% /md %}}
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L74"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> LocalSubjectAccessReview(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: inputApi.authorization.v1beta1.LocalSubjectAccessReview, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a authorization.v1beta1.LocalSubjectAccessReview resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L57">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#LocalSubjectAccessReview'>LocalSubjectAccessReview</a></pre>


Get the state of an existing `LocalSubjectAccessReview` resource, as identified by `id`.
Typically this ID  is of the form <namespace>/<name>; if <namespace> is omitted, then (per
Kubernetes convention) the ID becomes default/<name>.

Pulumi will keep track of this resource using `name` as the Pulumi ID.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L68">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of LocalSubjectAccessReview.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-apiVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L21">property <b>apiVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>apiVersion: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"authorization.k8s.io/v1beta1"</span>&gt;;</pre>
{{% md %}}

APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized
values. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#resources

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L138">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-kind">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L29">property <b>kind</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>kind: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"LocalSubjectAccessReview"</span>&gt;;</pre>
{{% md %}}

Kind is a string value representing the REST resource this object represents. Servers may
infer this from the endpoint the client submits requests to. Cannot be updated. In
CamelCase. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-metadata">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L32">property <b>metadata</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>metadata: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.meta.v1.ObjectMeta&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-spec">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L38">property <b>spec</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>spec: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectAccessReviewSpec&gt;;</pre>
{{% md %}}

Spec holds information about the request being evaluated.  spec.namespace must be equal to
the namespace you made the request against.  If empty, it is defaulted.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-status">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/LocalSubjectAccessReview.ts#L43">property <b>status</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>status: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectAccessReviewStatus&gt;;</pre>
{{% md %}}

Status is filled in by the server and indicates whether the request is allowed or not

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LocalSubjectAccessReview-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="SelfSubjectAccessReview">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L14">class <b>SelfSubjectAccessReview</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

SelfSubjectAccessReview checks whether or the current user can perform an action.  Not
filling in a spec.namespace means "in all namespaces".  Self is a special case, because users
should always be able to check whether they can perform an action

{{% /md %}}
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L73"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> SelfSubjectAccessReview(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: inputApi.authorization.v1beta1.SelfSubjectAccessReview, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a authorization.v1beta1.SelfSubjectAccessReview resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L56">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#SelfSubjectAccessReview'>SelfSubjectAccessReview</a></pre>


Get the state of an existing `SelfSubjectAccessReview` resource, as identified by `id`.
Typically this ID  is of the form <namespace>/<name>; if <namespace> is omitted, then (per
Kubernetes convention) the ID becomes default/<name>.

Pulumi will keep track of this resource using `name` as the Pulumi ID.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L67">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of SelfSubjectAccessReview.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-apiVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L21">property <b>apiVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>apiVersion: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"authorization.k8s.io/v1beta1"</span>&gt;;</pre>
{{% md %}}

APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized
values. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#resources

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L138">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-kind">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L29">property <b>kind</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>kind: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"SelfSubjectAccessReview"</span>&gt;;</pre>
{{% md %}}

Kind is a string value representing the REST resource this object represents. Servers may
infer this from the endpoint the client submits requests to. Cannot be updated. In
CamelCase. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-metadata">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L32">property <b>metadata</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>metadata: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.meta.v1.ObjectMeta&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-spec">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L37">property <b>spec</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>spec: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SelfSubjectAccessReviewSpec&gt;;</pre>
{{% md %}}

Spec holds information about the request being evaluated.  user and groups must be empty

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-status">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectAccessReview.ts#L42">property <b>status</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>status: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectAccessReviewStatus&gt;;</pre>
{{% md %}}

Status is filled in by the server and indicates whether the request is allowed or not

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectAccessReview-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="SelfSubjectRulesReview">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L19">class <b>SelfSubjectRulesReview</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

SelfSubjectRulesReview enumerates the set of actions the current user can perform within a
namespace. The returned list of actions may be incomplete depending on the server's
authorization mode, and any errors experienced during the evaluation. SelfSubjectRulesReview
should be used by UIs to show/hide actions, or to quickly let an end user reason about their
permissions. It should NOT Be used by external systems to drive authorization decisions as
this raises confused deputy, cache lifetime/revocation, and correctness concerns.
SubjectAccessReview, and LocalAccessReview are the correct way to defer authorization
decisions to the API server.

{{% /md %}}
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L78"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> SelfSubjectRulesReview(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: inputApi.authorization.v1beta1.SelfSubjectRulesReview, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a authorization.v1beta1.SelfSubjectRulesReview resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L61">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#SelfSubjectRulesReview'>SelfSubjectRulesReview</a></pre>


Get the state of an existing `SelfSubjectRulesReview` resource, as identified by `id`.
Typically this ID  is of the form <namespace>/<name>; if <namespace> is omitted, then (per
Kubernetes convention) the ID becomes default/<name>.

Pulumi will keep track of this resource using `name` as the Pulumi ID.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L72">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of SelfSubjectRulesReview.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-apiVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L26">property <b>apiVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>apiVersion: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"authorization.k8s.io/v1beta1"</span>&gt;;</pre>
{{% md %}}

APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized
values. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#resources

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L138">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-kind">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L34">property <b>kind</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>kind: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"SelfSubjectRulesReview"</span>&gt;;</pre>
{{% md %}}

Kind is a string value representing the REST resource this object represents. Servers may
infer this from the endpoint the client submits requests to. Cannot be updated. In
CamelCase. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-metadata">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L37">property <b>metadata</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>metadata: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.meta.v1.ObjectMeta&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-spec">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L42">property <b>spec</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>spec: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SelfSubjectRulesReviewSpec&gt;;</pre>
{{% md %}}

Spec holds information about the request being evaluated.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-status">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SelfSubjectRulesReview.ts#L47">property <b>status</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>status: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectRulesReviewStatus&gt;;</pre>
{{% md %}}

Status is filled in by the server and indicates the set of actions a user can perform.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SelfSubjectRulesReview-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="SubjectAccessReview">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L12">class <b>SubjectAccessReview</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

SubjectAccessReview checks whether or not a user or group can perform an action.

{{% /md %}}
<h3 class="pdoc-member-header" id="SubjectAccessReview-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L71"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> SubjectAccessReview(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: inputApi.authorization.v1beta1.SubjectAccessReview, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a authorization.v1beta1.SubjectAccessReview resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L54">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, opts?: <a href='/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#SubjectAccessReview'>SubjectAccessReview</a></pre>


Get the state of an existing `SubjectAccessReview` resource, as identified by `id`.
Typically this ID  is of the form <namespace>/<name>; if <namespace> is omitted, then (per
Kubernetes convention) the ID becomes default/<name>.

Pulumi will keep track of this resource using `name` as the Pulumi ID.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L65">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of SubjectAccessReview.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-apiVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L19">property <b>apiVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>apiVersion: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"authorization.k8s.io/v1beta1"</span>&gt;;</pre>
{{% md %}}

APIVersion defines the versioned schema of this representation of an object. Servers should
convert recognized schemas to the latest internal value, and may reject unrecognized
values. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#resources

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L138">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-kind">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L27">property <b>kind</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>kind: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='s2'>"SubjectAccessReview"</span>&gt;;</pre>
{{% md %}}

Kind is a string value representing the REST resource this object represents. Servers may
infer this from the endpoint the client submits requests to. Cannot be updated. In
CamelCase. More info:
https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-metadata">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L30">property <b>metadata</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>metadata: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.meta.v1.ObjectMeta&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-spec">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L35">property <b>spec</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>spec: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectAccessReviewSpec&gt;;</pre>
{{% md %}}

Spec holds information about the request being evaluated

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-status">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/authorization/v1beta1/SubjectAccessReview.ts#L40">property <b>status</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>status: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;outputApi.authorization.v1beta1.SubjectAccessReviewStatus&gt;;</pre>
{{% md %}}

Status is filled in by the server and indicates whether the request is allowed or not

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="SubjectAccessReview-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/7989847312c7a0b569453e0041b67b5d7506c7af/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>