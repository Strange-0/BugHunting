## Summary:
The blog site is vulnerable to reflected XSS in the search parameter. This vulnerability allows attackers to inject malicious scripts into the search query, which are then reflected back to users when they perform a search.

## Steps To Reproduce:

1. Go to https://blog.example.com/?s=<A HREF=https://attacker.com/>XSS-BY-STRANGE</A> Or Enter the payload manually in search box.
2. Payload Used :

```bash
 <A HREF=https://attacker.com/>XSS-BY-STRANGE</A>
```

##Screenshots:


## Impact

The presence of reflected XSS on the blog site introduces significant security risks. Attackers can craft malicious search queries containing scripts that, when executed, can steal user credentials, perform unauthorized actions on behalf of the user, or redirect them to malicious websites. Immediate attention is required to address this vulnerability and protect users from potential harm.
