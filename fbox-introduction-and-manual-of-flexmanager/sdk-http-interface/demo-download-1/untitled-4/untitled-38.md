# BoxCollectionArgs

盒子序列号或由接口返回的盒子ID，二选一

#### Inheritance

System.Object

BoxCollectionArgs

#### Inherited Members

System.Object.Equals\(System.Object\)

System.Object.Equals\(System.Object, System.Object\)

System.Object.GetHashCode\(\)

System.Object.GetType\(\)

System.Object.MemberwiseClone\(\)

System.Object.ReferenceEquals\(System.Object, System.Object\)

System.Object.ToString\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_BoxCollectionArgs_syntax"></a>

```text
public class BoxCollectionArgs
```

## Constructors <a id="constructors"></a>

### BoxCollectionArgs\(IReadOnlyList\) <a id="FBoxClientDriver_Contract_BoxCollectionArgs__ctor_System_Collections_Generic_IReadOnlyList_System_Int64__"></a>

#### Declaration

```text
public BoxCollectionArgs(IReadOnlyList boxIds)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IReadOnlyList&lt;System.Int64&gt; | boxIds |  |

### BoxCollectionArgs\(IReadOnlyList\) <a id="FBoxClientDriver_Contract_BoxCollectionArgs__ctor_System_Collections_Generic_IReadOnlyList_System_String__"></a>

#### Declaration

```text
public BoxCollectionArgs(IReadOnlyList boxNos)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Collections.Generic.IReadOnlyList&lt;System.String&gt; | boxNos |  |

## Properties <a id="properties"></a>

### BoxIds <a id="FBoxClientDriver_Contract_BoxCollectionArgs_BoxIds"></a>

#### Declaration

```text
public IReadOnlyList BoxIds { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IReadOnlyList&lt;System.Int64&gt; |  |

### BoxNos <a id="FBoxClientDriver_Contract_BoxCollectionArgs_BoxNos"></a>

#### Declaration

```text
public IReadOnlyList BoxNos { get; }
```

#### Property Value

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IReadOnlyList&lt;System.String&gt; |  |

