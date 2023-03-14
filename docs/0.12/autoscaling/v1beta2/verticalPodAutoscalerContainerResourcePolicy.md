---
permalink: /0.12/autoscaling/v1beta2/verticalPodAutoscalerContainerResourcePolicy/
---

# autoscaling.v1beta2.verticalPodAutoscalerContainerResourcePolicy

"An array of these is used as the input to `verticalPodAutoscaler.spec.resourcePolicy.withContainerPolicies()`."

## Index

* [`fn withContainerName(name)`](#fn-withcontainername)
* [`fn withControlledResources(resources)`](#fn-withcontrolledresources)
* [`fn withControlledResourcesMixin(resources)`](#fn-withcontrolledresourcesmixin)
* [`fn withControlledValues(values)`](#fn-withcontrolledvalues)
* [`fn withMaxAllowed(maxAllowed)`](#fn-withmaxallowed)
* [`fn withMaxAllowedMixin(maxAllowed)`](#fn-withmaxallowedmixin)
* [`fn withMinAllowed(maxAllowed)`](#fn-withminallowed)
* [`fn withMinAllowedMixin(minAllowed)`](#fn-withminallowedmixin)
* [`fn withMode(minAllowed)`](#fn-withmode)

## Fields

### fn withContainerName

```ts
withContainerName(name)
```

The name of the container that the policy applies to. If not specified, the policy serves as the default policy.

### fn withControlledResources

```ts
withControlledResources(resources)
```

Specifies the type of recommendations that will be computed (and possibly applied) by VPA. If not specified, the default of [ResourceCPU, ResourceMemory] will be used.

### fn withControlledResourcesMixin

```ts
withControlledResourcesMixin(resources)
```

withControlledResourcesMixin is like withControlledResources, but appends to the existing list

### fn withControlledValues

```ts
withControlledValues(values)
```

Which resource values should be controlled by VPA. Valid values are "RequestsAndLimits" and "RequestsOnly". The default is "RequestsAndLimits".

### fn withMaxAllowed

```ts
withMaxAllowed(maxAllowed)
```

Specifies the maximum amount of resources that will be recommended for the container. The default is no maximum.

### fn withMaxAllowedMixin

```ts
withMaxAllowedMixin(maxAllowed)
```

Like withMaxAllowed but merges with the existing object.

### fn withMinAllowed

```ts
withMinAllowed(maxAllowed)
```

Specifies the minimal amount of resources that will be recommended for the container. The default is no minimum.

### fn withMinAllowedMixin

```ts
withMinAllowedMixin(minAllowed)
```

Like withMinAllowed but merges with the existing object.

### fn withMode

```ts
withMode(minAllowed)
```

Whether autoscaler is enabled for the container. Valid values are "Off" and "Auto". The default is "Auto".