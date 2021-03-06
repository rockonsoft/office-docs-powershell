---
applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online
schema: 2.0.0
---

# Get-AddressBookPolicy

## SYNOPSIS
!!! Exchange Server 2010

Use the Get-AddressBookPolicy cmdlet to return address book policies that match the specified conditions.

!!! Exchange Server 2013

This cmdlet is available in on-premises Exchange and in the cloud-based service. Some parameters and settings may be exclusive to one environment or the other.

Use the Get-AddressBookPolicy cmdlet to return address book policies that match the specified conditions.

!!! Exchange Server 2016, Exchange Online

This cmdlet is available in on-premises Exchange and in the cloud-based service. Some parameters and settings may be exclusive to one environment or the other.

Use the Get-AddressBookPolicy cmdlet to return address book policies that match the specified conditions.

By default in Exchange Online, the Address List role isn't assigned to any role groups. To use any cmdlets that require the Address List role, you need to add the role to a role group. For more information, see the "Add a role to a role group" section in the topic, Manage role groups.

## SYNTAX

```
Get-AddressBookPolicy [[-Identity] <MailboxPolicyIdParameter>] [-DomainController <Fqdn>]
 [-Organization <OrganizationIdParameter>] [<CommonParameters>]
```

## DESCRIPTION
!!! Exchange Server 2010

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Address book policies" entry in the Mailbox Permissions topic.

!!! Exchange Server 2013

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Address book policies" entry in the Email address and address book permissions topic.

By default in Exchange Online, the Address List role isn't assigned to any role groups. To use any cmdlets that require the Address List role, you need to add the role to a role group. For more information, see the "Add a role to a role group" section in the topic, Manage role groups.

!!! Exchange Server 2016, Exchange Online

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see Find the permissions required to run any Exchange cmdlet (https://technet.microsoft.com/library/mt432940.aspx).

## EXAMPLES

### Example 1 -------------------------- (Exchange Server 2010)
```
Get-AddressBookPolicy | Format-List
```

This example returns detailed information about all address book policies in your organization by pipelining the Format-List cmdlet.

### Example 1 -------------------------- (Exchange Server 2013)
```
Get-AddressBookPolicy | Format-List
```

This example returns detailed information about all address book policies in your organization by pipelining the Format-List cmdlet.

### Example 1 -------------------------- (Exchange Server 2016)
```
Get-AddressBookPolicy | Format-List
```

This example returns detailed information about all address book policies in your organization by pipelining the Format-List cmdlet.

### Example 1 -------------------------- (Exchange Online)
```
Get-AddressBookPolicy | Format-List
```

This example returns detailed information about all address book policies in your organization by pipelining the Format-List cmdlet.

### Example 2 -------------------------- (Exchange Server 2010)
```
Get-AddressBookPolicy -Identity "All Fabrikam"
```

This example returns default information about the address book policy All Fabrikam

### Example 2 -------------------------- (Exchange Server 2013)
```
Get-AddressBookPolicy -Identity "All Fabrikam"
```

This example returns default information about the address book policy All Fabrikam

### Example 2 -------------------------- (Exchange Server 2016)
```
Get-AddressBookPolicy -Identity "All Fabrikam"
```

This example returns default information about the address book policy All Fabrikam

### Example 2 -------------------------- (Exchange Online)
```
Get-AddressBookPolicy -Identity "All Fabrikam"
```

This example returns default information about the address book policy All Fabrikam

### Example 2 -------------------------- (Exchange Server 2010)
```
Get-AddressBookPolicy | where {$_.OfflineAddressBook eq "\Fabrikam All OAB"}
```

This example returns information about all address book policies for which the offline address book (OAB) that the address book policy uses is named Fabrikam All OAB.

### Example 3 -------------------------- (Exchange Server 2013)
```
Get-AddressBookPolicy | where {$_.OfflineAddressBook eq "\Fabrikam All OAB"}
```

This example returns information about all address book policies for which the offline address book (OAB) that the address book policy uses is named Fabrikam All OAB.

### Example 3 -------------------------- (Exchange Server 2016)
```
Get-AddressBookPolicy | where {$_.OfflineAddressBook eq "\Fabrikam All OAB"}
```

This example returns information about all address book policies for which the offline address book (OAB) that the address book policy uses is named Fabrikam All OAB.

### Example 3 -------------------------- (Exchange Online)
```
Get-AddressBookPolicy | where {$_.OfflineAddressBook eq "\Fabrikam All OAB"}
```

This example returns information about all address book policies for which the offline address book (OAB) that the address book policy uses is named Fabrikam All OAB.

## PARAMETERS

### -Identity
The Identity parameter specifies the identity of the address book policy.

```yaml
Type: MailboxPolicyIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: 1
Default value: None
Accept pipeline input: True
Accept wildcard characters: False
```

### -DomainController
!!! Exchange Server 2010

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

This parameter is available only in on-premises Exchange.

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Organization
This parameter is available for multi-tenant deployments. It isn't available for on-premises deployments. For more information about multi-tenant deployments, see Multi-Tenant Support.

The Organization parameter specifies the organization in which you'll perform this action. This parameter doesn't accept wildcard characters, and you must use the exact name of the organization.

```yaml
Type: OrganizationIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  
To see the input types that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Input Type field for a cmdlet is blank, the cmdlet doesn't accept input data.

## OUTPUTS

###  
To see the return types, which are also known as output types, that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Output Type field is blank, the cmdlet doesn't return data.

## NOTES

## RELATED LINKS

[Online Version](https://technet.microsoft.com/library/a5ec362f-a941-454f-ba93-cecada3411db.aspx)

