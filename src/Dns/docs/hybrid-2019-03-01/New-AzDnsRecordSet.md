---
external help file:
Module Name: Az.Dns
online version: https://docs.microsoft.com/en-us/powershell/module/az.dns/new-azdnsrecordset
schema: 2.0.0
---

# New-AzDnsRecordSet

## SYNOPSIS
Creates or updates a record set within a DNS zone.

## SYNTAX

### CreateExpanded1 (Default)
```
New-AzDnsRecordSet -Name <String> -RecordType <RecordType> -ResourceGroupName <String>
 -SubscriptionId <String> -ZoneName <String> [-IfMatch <String>] [-IfNoneMatch <String>]
 [-ARecord <IARecord[]>] [-AaaaRecord <IAaaaRecord[]>] [-CnameRecordName <String>] [-Etag <String>]
 [-Id <String>] [-MXRecord <IMxRecord[]>] [-Metadata <Hashtable>] [-NSRecord <INsRecord[]>]
 [-PtrRecord <IPtrRecord[]>] [-ResourceName <String>] [-SoaRecordEmail <String>]
 [-SoaRecordExpireTime <Int64>] [-SoaRecordHost <String>] [-SoaRecordMinimumTtl <Int64>]
 [-SoaRecordRefreshTime <Int64>] [-SoaRecordRetryTime <Int64>] [-SoaRecordSerialNumber <Int64>]
 [-SrvRecord <ISrvRecord[]>] [-TimeToLive <Int64>] [-TxtRecord <ITxtRecord[]>] [-Type <String>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Create1
```
New-AzDnsRecordSet -Name <String> -RecordType <RecordType> -ResourceGroupName <String>
 -SubscriptionId <String> -ZoneName <String> -RecordSet <IRecordSet> [-IfMatch <String>]
 [-IfNoneMatch <String>] [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### CreateViaIdentityExpanded1
```
New-AzDnsRecordSet -InputObject <IDnsIdentity> [-IfMatch <String>] [-IfNoneMatch <String>]
 [-ARecord <IARecord[]>] [-AaaaRecord <IAaaaRecord[]>] [-CnameRecordName <String>] [-Etag <String>]
 [-Id <String>] [-MXRecord <IMxRecord[]>] [-Metadata <Hashtable>] [-NSRecord <INsRecord[]>]
 [-PtrRecord <IPtrRecord[]>] [-ResourceName <String>] [-SoaRecordEmail <String>]
 [-SoaRecordExpireTime <Int64>] [-SoaRecordHost <String>] [-SoaRecordMinimumTtl <Int64>]
 [-SoaRecordRefreshTime <Int64>] [-SoaRecordRetryTime <Int64>] [-SoaRecordSerialNumber <Int64>]
 [-SrvRecord <ISrvRecord[]>] [-TimeToLive <Int64>] [-TxtRecord <ITxtRecord[]>] [-Type <String>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### CreateViaIdentity1
```
New-AzDnsRecordSet -InputObject <IDnsIdentity> -RecordSet <IRecordSet> [-IfMatch <String>]
 [-IfNoneMatch <String>] [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Creates or updates a record set within a DNS zone.

## EXAMPLES

### Example 1: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

### Example 2: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

## PARAMETERS

### -AaaaRecord
The list of AAAA records in the record set.
To construct, see NOTES section for AAAARECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.IAaaaRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ARecord
The list of A records in the record set.
To construct, see NOTES section for ARECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.IARecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -CnameRecordName
The canonical name for this CNAME record.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Etag
The etag of the record set.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Id
The ID of the record set.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -IfMatch
The etag of the record set.
Omit this value to always overwrite the current record set.
Specify the last-seen etag value to prevent accidentally overwriting any concurrent changes.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -IfNoneMatch
Set to '*' to allow a new record set to be created, but to prevent updating an existing record set.
Other values will be ignored.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -InputObject
Identity Parameter

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.IDnsIdentity
Parameter Sets: CreateViaIdentityExpanded1, CreateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -Metadata
The metadata attached to the record set.

```yaml
Type: System.Collections.Hashtable
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -MXRecord
The list of MX records in the record set.
To construct, see NOTES section for MXRECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.IMxRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Name
The name of the record set, relative to the name of the zone.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, Create1
Aliases: RelativeRecordSetName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -NSRecord
The list of NS records in the record set.
To construct, see NOTES section for NSRECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.INsRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -PtrRecord
The list of PTR records in the record set.
To construct, see NOTES section for PTRRECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.IPtrRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -RecordSet
Describes a DNS record set (a collection of DNS records with the same name and type).
To construct, see NOTES section for RECORDSET properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20160401.IRecordSet
Parameter Sets: Create1, CreateViaIdentity1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -RecordType
The type of DNS record in this record set.
Record sets of type SOA can be updated but not created (they are created when the DNS zone is created).

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Support.RecordType
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ResourceGroupName
The name of the resource group.
The name is case insensitive.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, Create1
Aliases: Zone

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ResourceName
The name of the record set.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordEmail
The email contact for this SOA record.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordExpireTime
The expire time for this SOA record.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordHost
The domain name of the authoritative name server for this SOA record.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordMinimumTtl
The minimum value for this SOA record.
By convention this is used to determine the negative caching duration.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordRefreshTime
The refresh value for this SOA record.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordRetryTime
The retry time for this SOA record.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SoaRecordSerialNumber
The serial number for this SOA record.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SrvRecord
The list of SRV records in the record set.
To construct, see NOTES section for SRVRECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.ISrvRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SubscriptionId
The ID of the target subscription.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -TimeToLive
The TTL (time-to-live) of the records in the record set.

```yaml
Type: System.Int64
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases: Ttl

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -TxtRecord
The list of TXT records in the record set.
To construct, see NOTES section for TXTRECORD properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20150504Preview.ITxtRecord[]
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Type
The type of the record set.

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, CreateViaIdentityExpanded1
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ZoneName
The name of the DNS zone (without a terminating dot).

```yaml
Type: System.String
Parameter Sets: CreateExpanded1, Create1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.IDnsIdentity

### Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20160401.IRecordSet

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Dns.Models.Api20160401.IRecordSet

## ALIASES

## NOTES

### COMPLEX PARAMETER PROPERTIES
To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.

#### AAAARECORD <IAaaaRecord[]>: The list of AAAA records in the record set.
  - `[Ipv6Address <String>]`: The IPv6 address of this AAAA record.

#### ARECORD <IARecord[]>: The list of A records in the record set.
  - `[Ipv4Address <String>]`: The IPv4 address of this A record.

#### MXRECORD <IMxRecord[]>: The list of MX records in the record set.
  - `[Exchange <String>]`: The domain name of the mail host for this MX record.
  - `[Preference <Int32?>]`: The preference value for this MX record.

#### NSRECORD <INsRecord[]>: The list of NS records in the record set.
  - `[Nsdname <String>]`: The name server name for this NS record.

#### PTRRECORD <IPtrRecord[]>: The list of PTR records in the record set.
  - `[Ptrdname <String>]`: The PTR target domain name for this PTR record.

#### RECORDSET <IRecordSet>: Describes a DNS record set (a collection of DNS records with the same name and type).
  - `[ARecord <IARecord[]>]`: The list of A records in the record set.
    - `[Ipv4Address <String>]`: The IPv4 address of this A record.
  - `[AaaaRecord <IAaaaRecord[]>]`: The list of AAAA records in the record set.
    - `[Ipv6Address <String>]`: The IPv6 address of this AAAA record.
  - `[CnameRecordCname <String>]`: The canonical name for this CNAME record.
  - `[Etag <String>]`: The etag of the record set.
  - `[Id <String>]`: The ID of the record set.
  - `[Metadata <IRecordSetPropertiesMetadata>]`: The metadata attached to the record set.
    - `[(Any) <String>]`: This indicates any property can be added to this object.
  - `[MxRecord <IMxRecord[]>]`: The list of MX records in the record set.
    - `[Exchange <String>]`: The domain name of the mail host for this MX record.
    - `[Preference <Int32?>]`: The preference value for this MX record.
  - `[Name <String>]`: The name of the record set.
  - `[NsRecord <INsRecord[]>]`: The list of NS records in the record set.
    - `[Nsdname <String>]`: The name server name for this NS record.
  - `[PtrRecord <IPtrRecord[]>]`: The list of PTR records in the record set.
    - `[Ptrdname <String>]`: The PTR target domain name for this PTR record.
  - `[SoaRecordEmail <String>]`: The email contact for this SOA record.
  - `[SoaRecordExpireTime <Int64?>]`: The expire time for this SOA record.
  - `[SoaRecordHost <String>]`: The domain name of the authoritative name server for this SOA record.
  - `[SoaRecordMinimumTtl <Int64?>]`: The minimum value for this SOA record. By convention this is used to determine the negative caching duration.
  - `[SoaRecordRefreshTime <Int64?>]`: The refresh value for this SOA record.
  - `[SoaRecordRetryTime <Int64?>]`: The retry time for this SOA record.
  - `[SoaRecordSerialNumber <Int64?>]`: The serial number for this SOA record.
  - `[SrvRecord <ISrvRecord[]>]`: The list of SRV records in the record set.
    - `[Port <Int32?>]`: The port value for this SRV record.
    - `[Priority <Int32?>]`: The priority value for this SRV record.
    - `[Target <String>]`: The target domain name for this SRV record.
    - `[Weight <Int32?>]`: The weight value for this SRV record.
  - `[Ttl <Int64?>]`: The TTL (time-to-live) of the records in the record set.
  - `[TxtRecord <ITxtRecord[]>]`: The list of TXT records in the record set.
    - `[Value <String[]>]`: The text value of this TXT record.
  - `[Type <String>]`: The type of the record set.

#### SRVRECORD <ISrvRecord[]>: The list of SRV records in the record set.
  - `[Port <Int32?>]`: The port value for this SRV record.
  - `[Priority <Int32?>]`: The priority value for this SRV record.
  - `[Target <String>]`: The target domain name for this SRV record.
  - `[Weight <Int32?>]`: The weight value for this SRV record.

#### TXTRECORD <ITxtRecord[]>: The list of TXT records in the record set.
  - `[Value <String[]>]`: The text value of this TXT record.

## RELATED LINKS
