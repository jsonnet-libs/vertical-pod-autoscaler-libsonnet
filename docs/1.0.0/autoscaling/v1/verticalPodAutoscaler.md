---
permalink: /1.0.0/autoscaling/v1/verticalPodAutoscaler/
---

# autoscaling.v1.verticalPodAutoscaler

"VerticalPodAutoscaler is the configuration for a vertical pod autoscaler, which automatically manages pod resources based on historical and real time resource utilization."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withRecommenders(recommenders)`](#fn-specwithrecommenders)
  * [`fn withRecommendersMixin(recommenders)`](#fn-specwithrecommendersmixin)
  * [`fn withTargetRef(object)`](#fn-specwithtargetref)
  * [`obj spec.recommenders`](#obj-specrecommenders)
    * [`fn withName(name)`](#fn-specrecommenderswithname)
  * [`obj spec.resourcePolicy`](#obj-specresourcepolicy)
    * [`fn withContainerPolicies(containerPolicies)`](#fn-specresourcepolicywithcontainerpolicies)
    * [`fn withContainerPoliciesMixin(containerPolicies)`](#fn-specresourcepolicywithcontainerpoliciesmixin)
    * [`obj spec.resourcePolicy.containerPolicies`](#obj-specresourcepolicycontainerpolicies)
      * [`fn withContainerName(containerName)`](#fn-specresourcepolicycontainerpolicieswithcontainername)
      * [`fn withControlledResources(controlledResources)`](#fn-specresourcepolicycontainerpolicieswithcontrolledresources)
      * [`fn withControlledResourcesMixin(controlledResources)`](#fn-specresourcepolicycontainerpolicieswithcontrolledresourcesmixin)
      * [`fn withControlledValues(controlledValues)`](#fn-specresourcepolicycontainerpolicieswithcontrolledvalues)
      * [`fn withMaxAllowed(maxAllowed)`](#fn-specresourcepolicycontainerpolicieswithmaxallowed)
      * [`fn withMaxAllowedMixin(maxAllowed)`](#fn-specresourcepolicycontainerpolicieswithmaxallowedmixin)
      * [`fn withMinAllowed(minAllowed)`](#fn-specresourcepolicycontainerpolicieswithminallowed)
      * [`fn withMinAllowedMixin(minAllowed)`](#fn-specresourcepolicycontainerpolicieswithminallowedmixin)
      * [`fn withMode(mode)`](#fn-specresourcepolicycontainerpolicieswithmode)
  * [`obj spec.targetRef`](#obj-spectargetref)
    * [`fn withApiVersion(apiVersion)`](#fn-spectargetrefwithapiversion)
    * [`fn withKind(kind)`](#fn-spectargetrefwithkind)
    * [`fn withName(name)`](#fn-spectargetrefwithname)
  * [`obj spec.updatePolicy`](#obj-specupdatepolicy)
    * [`fn withEvictionRequirements(evictionRequirements)`](#fn-specupdatepolicywithevictionrequirements)
    * [`fn withEvictionRequirementsMixin(evictionRequirements)`](#fn-specupdatepolicywithevictionrequirementsmixin)
    * [`fn withMinReplicas(minReplicas)`](#fn-specupdatepolicywithminreplicas)
    * [`fn withUpdateMode(updateMode)`](#fn-specupdatepolicywithupdatemode)
    * [`obj spec.updatePolicy.evictionRequirements`](#obj-specupdatepolicyevictionrequirements)
      * [`fn withChangeRequirement(changeRequirement)`](#fn-specupdatepolicyevictionrequirementswithchangerequirement)
      * [`fn withResource(resource)`](#fn-specupdatepolicyevictionrequirementswithresource)
      * [`fn withResourceMixin(resource)`](#fn-specupdatepolicyevictionrequirementswithresourcemixin)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of VerticalPodAutoscaler

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"Specification of the behavior of the autoscaler. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status."

### fn spec.withRecommenders

```ts
withRecommenders(recommenders)
```

"Recommender responsible for generating recommendation for this object. List should be empty (then the default recommender will generate the recommendation) or contain exactly one recommender."

### fn spec.withRecommendersMixin

```ts
withRecommendersMixin(recommenders)
```

"Recommender responsible for generating recommendation for this object. List should be empty (then the default recommender will generate the recommendation) or contain exactly one recommender."

**Note:** This function appends passed data to existing values

### fn spec.withTargetRef

```ts
withTargetRef(object)
```

Set spec.TargetRef to `object`

## obj spec.recommenders

"Recommender responsible for generating recommendation for this object. List should be empty (then the default recommender will generate the recommendation) or contain exactly one recommender."

### fn spec.recommenders.withName

```ts
withName(name)
```

"Name of the recommender responsible for generating recommendation for this object."

## obj spec.resourcePolicy

"Controls how the autoscaler computes recommended resources. The resource policy may be used to set constraints on the recommendations for individual containers. If not specified, the autoscaler computes recommended resources for all containers in the pod, without additional constraints."

### fn spec.resourcePolicy.withContainerPolicies

```ts
withContainerPolicies(containerPolicies)
```

"Per-container resource policies."

### fn spec.resourcePolicy.withContainerPoliciesMixin

```ts
withContainerPoliciesMixin(containerPolicies)
```

"Per-container resource policies."

**Note:** This function appends passed data to existing values

## obj spec.resourcePolicy.containerPolicies

"Per-container resource policies."

### fn spec.resourcePolicy.containerPolicies.withContainerName

```ts
withContainerName(containerName)
```

"Name of the container or DefaultContainerResourcePolicy, in which case the policy is used by the containers that don't have their own policy specified."

### fn spec.resourcePolicy.containerPolicies.withControlledResources

```ts
withControlledResources(controlledResources)
```

"Specifies the type of recommendations that will be computed (and possibly applied) by VPA. If not specified, the default of [ResourceCPU, ResourceMemory] will be used."

### fn spec.resourcePolicy.containerPolicies.withControlledResourcesMixin

```ts
withControlledResourcesMixin(controlledResources)
```

"Specifies the type of recommendations that will be computed (and possibly applied) by VPA. If not specified, the default of [ResourceCPU, ResourceMemory] will be used."

**Note:** This function appends passed data to existing values

### fn spec.resourcePolicy.containerPolicies.withControlledValues

```ts
withControlledValues(controlledValues)
```

"Specifies which resource values should be controlled. The default is \"RequestsAndLimits\"."

### fn spec.resourcePolicy.containerPolicies.withMaxAllowed

```ts
withMaxAllowed(maxAllowed)
```

"Specifies the maximum amount of resources that will be recommended for the container. The default is no maximum."

### fn spec.resourcePolicy.containerPolicies.withMaxAllowedMixin

```ts
withMaxAllowedMixin(maxAllowed)
```

"Specifies the maximum amount of resources that will be recommended for the container. The default is no maximum."

**Note:** This function appends passed data to existing values

### fn spec.resourcePolicy.containerPolicies.withMinAllowed

```ts
withMinAllowed(minAllowed)
```

"Specifies the minimal amount of resources that will be recommended for the container. The default is no minimum."

### fn spec.resourcePolicy.containerPolicies.withMinAllowedMixin

```ts
withMinAllowedMixin(minAllowed)
```

"Specifies the minimal amount of resources that will be recommended for the container. The default is no minimum."

**Note:** This function appends passed data to existing values

### fn spec.resourcePolicy.containerPolicies.withMode

```ts
withMode(mode)
```

"Whether autoscaler is enabled for the container. The default is \"Auto\"."

## obj spec.targetRef

"TargetRef points to the controller managing the set of pods for the autoscaler to control - e.g. Deployment, StatefulSet. VerticalPodAutoscaler can be targeted at controller implementing scale subresource (the pod set is retrieved from the controller's ScaleStatus) or some well known controllers (e.g. for DaemonSet the pod set is read from the controller's spec). If VerticalPodAutoscaler cannot use specified target it will report ConfigUnsupported condition. Note that VerticalPodAutoscaler does not require full implementation of scale subresource - it will not use it to modify the replica count. The only thing retrieved is a label selector matching pods grouped by the target resource."

### fn spec.targetRef.withApiVersion

```ts
withApiVersion(apiVersion)
```

"API version of the referent"

### fn spec.targetRef.withKind

```ts
withKind(kind)
```

"Kind of the referent; More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds"

### fn spec.targetRef.withName

```ts
withName(name)
```

"Name of the referent; More info: http://kubernetes.io/docs/user-guide/identifiers#names"

## obj spec.updatePolicy

"Describes the rules on how changes are applied to the pods. If not specified, all fields in the `PodUpdatePolicy` are set to their default values."

### fn spec.updatePolicy.withEvictionRequirements

```ts
withEvictionRequirements(evictionRequirements)
```

"EvictionRequirements is a list of EvictionRequirements that need to evaluate to true in order for a Pod to be evicted. If more than one EvictionRequirement is specified, all of them need to be fulfilled to allow eviction."

### fn spec.updatePolicy.withEvictionRequirementsMixin

```ts
withEvictionRequirementsMixin(evictionRequirements)
```

"EvictionRequirements is a list of EvictionRequirements that need to evaluate to true in order for a Pod to be evicted. If more than one EvictionRequirement is specified, all of them need to be fulfilled to allow eviction."

**Note:** This function appends passed data to existing values

### fn spec.updatePolicy.withMinReplicas

```ts
withMinReplicas(minReplicas)
```

"Minimal number of replicas which need to be alive for Updater to attempt pod eviction (pending other checks like PDB). Only positive values are allowed. Overrides global '--min-replicas' flag."

### fn spec.updatePolicy.withUpdateMode

```ts
withUpdateMode(updateMode)
```

"Controls when autoscaler applies changes to the pod resources. The default is 'Auto'."

## obj spec.updatePolicy.evictionRequirements

"EvictionRequirements is a list of EvictionRequirements that need to evaluate to true in order for a Pod to be evicted. If more than one EvictionRequirement is specified, all of them need to be fulfilled to allow eviction."

### fn spec.updatePolicy.evictionRequirements.withChangeRequirement

```ts
withChangeRequirement(changeRequirement)
```

"EvictionChangeRequirement refers to the relationship between the new target recommendation for a Pod and its current requests, what kind of change is necessary for the Pod to be evicted"

### fn spec.updatePolicy.evictionRequirements.withResource

```ts
withResource(resource)
```

"Resources is a list of one or more resources that the condition applies to. If more than one resource is given, the EvictionRequirement is fulfilled if at least one resource meets `changeRequirement`."

### fn spec.updatePolicy.evictionRequirements.withResourceMixin

```ts
withResourceMixin(resource)
```

"Resources is a list of one or more resources that the condition applies to. If more than one resource is given, the EvictionRequirement is fulfilled if at least one resource meets `changeRequirement`."

**Note:** This function appends passed data to existing values