# Clan Verification Tutorial

The clan verification system is designed to aid in adding roles for new clan members. Instead of having to ping a server moderator to give you the clan role, the bot can do it for you.

## Table of Contents

 - [Setup](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#setup)
 - [Setup Examples](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#setup-examples)
   - [Simple](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#simple)
   - [Separate Ranks](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#separate-ranks)
   - [Common Ranks](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#seperate-ranks)
   - [No General](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#seperate-ranks)
   - [Multiclan Combined](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#multiclan-combined)
   - [Multiclan Complex](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#multiclan-complex)
   - [Footnote](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#footnote)
 - [Delete vs. Delete Force](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#delete-vs-delete-force)
 - [FAQ](https://github.com/PixellProton/Karutwo/blob/main/tutorials/clan-verification.md#faq)

## Setup

You must have the `Manage server` permission to set up **your clan** on the server the command is run in. This means that **multiple shoguns** can set up in a single server. Here are the roles you can set:
 - **General role 1 and 2**: these roles will be added to every member, no matter the rank.
 - **Rank roles**: these roles will be added to the corresponding rank (i.e. Tairos get the Tairo rank)

If you use setup in a server that already has your clan setup, it will overwrite. However, if you use setup in a server while another server has your clan setup, you must delete it first with `/clan delete`.

## Setup Examples

### Simple
general_role_1:`@Clan Member`
> Everyone gets `@Clan Member`

### Separate Ranks
general_role_1:`@Clan Member`, tairo_role:`@Tairo`, roju_role:`@Roju`
> Everyone gets `@Clan Member`  
> Tairos get `@Tairo`  
> Rojus get `@Roju`  

### Common Ranks
general_role_1:`@Clan Member`, tairo_role:`@Giveaway Host`, roju_role:`@Giveaway Host`
> Everyone gets `@Clan Member`  
> Tairos and Rojus get `@Giveaway Host`  

### No General
tairo_role:`@Giveaway Host`, roju_role:`@Giveaway Host`
> Tairos and Rojus get `@Giveaway Host`  

### Multiclan Combined
**Proton's Clan**: general_role_1:`@Clan Member`  
**Electron's Clan**: general_role_1:`@Clan Member`
> Everyone gets `@Clan Member`

### Multiclan Complex
**Proton's Clan**: general_role_1:`@Clan Member`, general_role_2:`@Proton Clan`    
**Electron's Clan**: general_role_1:`@Clan Member`, general_role_2:`@Electron Clan`  
> Everyone gets `@Clan Member`  
> Proton's Clan gets `@Proton Clan`  
> Electron's Clan gets `@Electron Clan`

### Footnote
These are merely a few examples of combinations. You can mix and match combinations. For example Multiclan Complex + Seperate Ranks = general roles follow Multiclan Complex while rank roles follow Seperate Ranks.

## Delete vs. Delete Force

Most of times, you'll only need to use `/clan delete`. Regular delete removes **your** clan verification setup from the server. However, if a shogun deletes their Discord account or refuses to delete their clan from your server, you can force delete their clan. 

## FAQ

**Is it possible to have multiple clans in the same server?**
> Yes. However, only the shoguns must need the `Manage server` permission and can only manage their own clan.

**Is there a limit to how many clans are allowed in the same server?**
> Yes, 8. However, if you need more, please DM me `PixellProton#8577` at or ping me in the [support server](https://discord.gg/9r9pczygG8).

**A shogun in my server refuses to delete their clan, what can I do about it?**
> If you have the `Manage server` permission, yuo can use `/clan delete-force` to remove their clan. You should also remove the `Manage server` permission from the shogun so they don't setup again.
