---
title: "Module types/input"
linktitle: "input"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->






<h3>APIs</h3>
<ul class="api">
    <li><a href="#ProjectSharedWithGroup"><span class="symbol api"></span>ProjectSharedWithGroup</a></li>
</ul>




<h2 id="apis">APIs</h2>
<h3 class="pdoc-module-header" id="ProjectSharedWithGroup" data-link-title="ProjectSharedWithGroup">
    <a href="https://github.com/pulumi/pulumi-gitlab/blob/028b061a7ff4237d00706de80d79c333ab5cf8eb/sdk/nodejs/types/input.ts#L7">
        interface <strong>ProjectSharedWithGroup</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ProjectSharedWithGroup</span></code></pre>
<h4 class="pdoc-member-header" id="ProjectSharedWithGroup-groupAccessLevel">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gitlab/blob/028b061a7ff4237d00706de80d79c333ab5cf8eb/sdk/nodejs/types/input.ts#L12">property <b>groupAccessLevel</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>groupAccessLevel: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Group's sharing permissions. See [group members permission][groupMembersPermissions] for more info.
Valid values are `guest`, `reporter`, `developer`, `master`.

<h4 class="pdoc-member-header" id="ProjectSharedWithGroup-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gitlab/blob/028b061a7ff4237d00706de80d79c333ab5cf8eb/sdk/nodejs/types/input.ts#L16">property <b>groupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>groupId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</code></pre>

Group id of the group you want to share the project with.

<h4 class="pdoc-member-header" id="ProjectSharedWithGroup-groupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gitlab/blob/028b061a7ff4237d00706de80d79c333ab5cf8eb/sdk/nodejs/types/input.ts#L20">property <b>groupName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>groupName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Group's name.
