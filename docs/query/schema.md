pr## GraphQL Schema

The PPQ schema is modelled after schema.net; all available types and queries are listed here.

# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Objects](#objects)
    * [Article](#article)
    * [ArticleQuery](#articlequery)
    * [Audience](#audience)
    * [Author](#author)
    * [CookingMethod](#cookingmethod)
    * [CreativeWorkQuery](#creativeworkquery)
    * [DirectoryService](#directoryservice)
    * [DoseSchedule](#doseschedule)
    * [Drug](#drug)
    * [Energy](#energy)
    * [GeoCoordinatesQuery](#geocoordinatesquery)
    * [HowTo](#howto)
    * [Hub](#hub)
    * [HubVideo](#hubvideo)
    * [MarkdownField](#markdownfield)
    * [Markup](#markup)
    * [Mass](#mass)
    * [MaximumDose](#maximumdose)
    * [MediaField](#mediafield)
    * [MedicalArticle](#medicalarticle)
    * [MedicalCode](#medicalcode)
    * [MedicalCondition](#medicalcondition)
    * [MedicalDrugArticle](#medicaldrugarticle)
    * [MedicalEntity](#medicalentity)
    * [MedicalIndication](#medicalindication)
    * [MedicalProcedure](#medicalprocedure)
    * [MedicalSignOrSymptom](#medicalsignorsymptom)
    * [MedicalSpeciality](#medicalspeciality)
    * [MedicalTherapy](#medicaltherapy)
    * [MedicalWebpage](#medicalwebpage)
    * [NutritionalInformation](#nutritionalinformation)
    * [Offer](#offer)
    * [Organization](#organization)
    * [OrganizationQuery](#organizationquery)
    * [PeopleAudience](#peopleaudience)
    * [PersonQuery](#personquery)
    * [Place](#place)
    * [PostalAddress](#postaladdress)
    * [PriceSpecificationQuery](#pricespecificationquery)
    * [PropertyValue](#propertyvalue)
    * [Quantity](#quantity)
    * [Recipe](#recipe)
    * [RecipeIngredient](#recipeingredient)
    * [RecipeQuery](#recipequery)
    * [SearchPromotion](#searchpromotion)
    * [SearchResult](#searchresult)
    * [ServiceQuery](#servicequery)
    * [Substance](#substance)
    * [TherapeuticProcedure](#therapeuticprocedure)
    * [Thing](#thing)
    * [Webpage](#webpage)
  * [Inputs](#inputs)
    * [ArticleInput](#articleinput)
    * [ArticleOrderByInput](#articleorderbyinput)
    * [ArticleWhereInput](#articlewhereinput)
    * [AuthorOrderByInput](#authororderbyinput)
    * [AuthorWhereInput](#authorwhereinput)
    * [DirectoryServiceOrderByInput](#directoryserviceorderbyinput)
    * [DirectoryServiceWhereInput](#directoryservicewhereinput)
    * [HubOrderByInput](#huborderbyinput)
    * [HubWhereInput](#hubwhereinput)
    * [MedicalArticleOrderByInput](#medicalarticleorderbyinput)
    * [MedicalArticleWhereInput](#medicalarticlewhereinput)
    * [MedicalConditionPartInput](#medicalconditionpartinput)
    * [MedicalDrugArticleOrderByInput](#medicaldrugarticleorderbyinput)
    * [MedicalDrugArticleWhereInput](#medicaldrugarticlewhereinput)
    * [MedicalEntityPartInput](#medicalentitypartinput)
    * [MedicalWebpagePartInput](#medicalwebpagepartinput)
    * [OrganizationOrderByInput](#organizationorderbyinput)
    * [OrganizationWhereInput](#organizationwhereinput)
    * [RecipeOrderByInput](#recipeorderbyinput)
    * [RecipePartInput](#recipepartinput)
    * [RecipeWhereInput](#recipewhereinput)
    * [WebpagePartInput](#webpagepartinput)
  * [Enums](#enums)
    * [DosageForm](#dosageform)
    * [OrderByDirection](#orderbydirection)
    * [PrescriptionStatus](#prescriptionstatus)
    * [RecipeDifficulty](#recipedifficulty)
    * [ServingUnit](#servingunit)
    * [Status](#status)
    * [UrlKind](#urlkind)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [Date](#date)
    * [DateTime](#datetime)
    * [DateTimeOffset](#datetimeoffset)
    * [Decimal](#decimal)
    * [Float](#float)
    * [ID](#id)
    * [Int](#int)
    * [Milliseconds](#milliseconds)
    * [Seconds](#seconds)
    * [String](#string)
    * [Uri](#uri)

</details>

## Query
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>article</strong></td>
<td valign="top">[<a href="#article">Article</a>]</td>
<td>

Represents a Article.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#articlewhereinput">ArticleWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#articleorderbyinput">ArticleOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#author">Author</a>]</td>
<td>

Represents a Author.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#authorwhereinput">AuthorWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#authororderbyinput">AuthorOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItem</strong></td>
<td valign="top"><a href="#contentitem">ContentItem</a></td>
<td>

Content items are instances of content types, just like objects are instances of classes.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">contentItemId</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Content item id

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>directoryService</strong></td>
<td valign="top">[<a href="#directoryservice">DirectoryService</a>]</td>
<td>

Represents a Directory Service.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#directoryservicewhereinput">DirectoryServiceWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#directoryserviceorderbyinput">DirectoryServiceOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hub</strong></td>
<td valign="top">[<a href="#hub">Hub</a>]</td>
<td>

Represents a Hub.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#hubwhereinput">HubWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#huborderbyinput">HubOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalArticle</strong></td>
<td valign="top">[<a href="#medicalarticle">MedicalArticle</a>]</td>
<td>

Represents a Medical Article.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#medicalarticlewhereinput">MedicalArticleWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#medicalarticleorderbyinput">MedicalArticleOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalDrugArticle</strong></td>
<td valign="top">[<a href="#medicaldrugarticle">MedicalDrugArticle</a>]</td>
<td>

Represents a Medical Drug Article.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#medicaldrugarticlewhereinput">MedicalDrugArticleWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#medicaldrugarticleorderbyinput">MedicalDrugArticleOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organization</strong></td>
<td valign="top">[<a href="#organization">Organization</a>]</td>
<td>

Represents a Organization.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#organizationwhereinput">OrganizationWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#organizationorderbyinput">OrganizationOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recipe</strong></td>
<td valign="top">[<a href="#recipe">Recipe</a>]</td>
<td>

Represents a Recipe.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#recipewhereinput">RecipeWhereInput</a></td>
<td>

filters the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">orderBy</td>
<td valign="top"><a href="#recipeorderbyinput">RecipeOrderByInput</a></td>
<td>

sort order

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of content items to skip

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">status</td>
<td valign="top"><a href="#status">Status</a></td>
<td>

publication status of the content item

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>search</strong></td>
<td valign="top"><a href="#searchresult">SearchResult</a></td>
<td>

Provides search functionality over content.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">term</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The search term

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">collections</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A list of collections to search across.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Records to skip.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">take</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Records to take.

</td>
</tr>
</tbody>
</table>

## Objects

### Article

Represents a Article.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### ArticleQuery

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>articleBody</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The actual body of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>wordCount</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The number of words in the text of the Article.

</td>
</tr>
</tbody>
</table>

### Audience

Intended audience for an item, i.e. the group for whom the item was created.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audienceType</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The target group associated with a given audience (e.g. patients, medical professionals, etc.).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>geographicArea</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The geographic area associated with the audience.

</td>
</tr>
</tbody>
</table>

### Author

Represents a Author.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>accrediation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>additionalName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An additional name for a Person, can be used for a middle name.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Physical address of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>affiliation</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An organization that this person is affiliated with. For example, a school/university, a club, or a team.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alumniOf</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An organization that the person is an alumni of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>biography</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>birthDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

Date of birth.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>currentVersionAuthor</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Email address.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>familyName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Family name. In the U.S., the last name of an Person. This can be used along with givenName instead of the name property.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Gender of the person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>givenName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Given name. In the U.S., the first name of a Person. This can be used along with familyName instead of the name property.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>honorificPrefix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An honorific prefix preceding a Person's name such as Dr/Mrs/Mr.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>honorificSuffix</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

An honorific suffix preceding a Person's name such as M.D. /PhD/MSCSW.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

An image of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>jobTitle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The job title of the person (for example, Financial Manager).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>memberOf</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An Organization to which this Person or Organization belongs.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nationality</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Nationality of the person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>peerReviewer</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shortBiography</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>telephoneNumber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The telephone number.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>worksFor</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

Organizations that the person works for.

</td>
</tr>
</tbody>
</table>

### CookingMethod

The method of cooking, such as Frying, Steaming, ...

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>method</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The method of cooking, such as Frying, Steaming, ...

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>methodCaption</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A short caption to help idenify the method.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>methodImageUrl</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

An image url descriping the method.

</td>
</tr>
</tbody>
</table>

### CreativeWorkQuery

The most generic kind of creative work, including books, movies, photographs, software programs, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quotation</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The (e.g. fictional) character, Person or Organization to whom the quotation is attributed within the containing CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### DirectoryService

Represents a Directory Service.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
</tbody>
</table>

### DoseSchedule

A specific dosing schedule for a drug or supplement.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>doseUnit</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The unit of the dose, e.g. 'mg'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>doseValue</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The value of the dose, e.g. 500.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>frequency</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

How often the dose is taken, e.g. 'daily'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>targetPopulation</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Characteristics of the population for which this is intended, or which typically uses it, e.g. 'adults'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Drug

A chemical or biologic substance, used as a medical therapy, that has a physiological effect on an organism. Here the term drug is used interchangeably with the term medicine although clinical knowledge make a clear difference between them.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>activeIngredient</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An active ingredient, typically chemical compounds and/or biologic substances.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>administrationRoute</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

	A route by which this drug may be administered, e.g. 'oral'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alcoholWarning</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any precaution, guidance, contraindication, etc. related to consumption of alcohol while taking this drug.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>breastfeedingWarning</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any precaution, guidance, contraindication, etc. related to this drug's use by breastfeeding mothers.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clinicalPharmacology</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Description of the absorption and elimination of drugs, including their concentration (pharmacokinetics, pK) and biological effects (pharmacodynamics, pD).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosageForm</strong></td>
<td valign="top"><a href="#dosageform">DosageForm</a></td>
<td>

A dosage form in which this drug/supplement is available, e.g. 'tablet', 'suspension', 'injection'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drugUnit</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The unit in which the drug is measured, e.g. '5 mg tablet'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foodWarning</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any precaution, guidance, contraindication, etc. related to consumption of specific foods while taking this drug.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isAvailableGenerically</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

True if the drug is available in a generic form (regardless of name).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isProprietary</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

True if this item's name is a proprietary/brand name (vs. generic name).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mechanismOfAction</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The specific biochemical interaction through which this drug or supplement produces its pharmacological effect.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nonProprietaryName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The generic name of this drug or supplement.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>overdosage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any information related to overdose on a drug, including signs or symptoms, treatments, contact information for emergency response.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pregnancyWarning</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any precaution, guidance, contraindication, etc. related to this drug's use during pregnancy.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribingInfo</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

Link to prescribing information for the drug.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptionStatus</strong></td>
<td valign="top"><a href="#prescriptionstatus">PrescriptionStatus</a></td>
<td>

Indicates the status of drug prescription eg. local catalogs classifications or whether the drug is available by prescription or over-the-counter, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>proprietaryName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Proprietary name given to the diet plan, typically by its originator or creator.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relatedDrug</strong></td>
<td valign="top">[<a href="#drug">Drug</a>]</td>
<td>

Any other drug related to this one, for example commonly-prescribed alternatives.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rXCUI</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The RxCUI drug identifier from RXNORM.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warning</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Any FDA or other warnings about the drug (text or URL).

</td>
</tr>
</tbody>
</table>

### Energy

Properties that take Energy as values are of the form '<Number> <Energy unit of measure>'.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>measurment</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The measurment, such as Kg or mm.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>number</strong></td>
<td valign="top"><a href="#decimal">Decimal</a>!</td>
<td>

The value.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### GeoCoordinatesQuery

The geographic coordinates of a place or event.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#postaladdress">PostalAddress</a></td>
<td>

Physical address of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressCountry</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The country. For example, USA. You can also provide the two-letter ISO 3166-1 alpha-2 country code.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>elevation</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The elevation of a location (WGS 84).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The latitude of a location. For example 37.42242 (WGS 84).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>longitude</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The longitude of a location. For example -122.08585 (WGS 84).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postalCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The postal code. For example, 94043.

</td>
</tr>
</tbody>
</table>

### HowTo

Instructions that explain how to achieve a result by performing a sequence of steps.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>step</strong></td>
<td valign="top">[<a href="#creativeworkquery">CreativeWorkQuery</a>]</td>
<td>

A single step item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>supply</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A sub-property of instrument. A supply consumed when performing instructions or a direction.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>yield</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The quantity that results by performing instructions. For example, a paper airplane, 10 personalized candles.

</td>
</tr>
</tbody>
</table>

### HtmlBodyPart

Content stored as HTML.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>html</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### Hub

Represents a Hub.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### HubVideo

A Video, describe the caption, description, quality, frame size and type of the video, ...

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>caption</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A video caption describe the title of the video.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>embedUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A URL pointing to a player for a specific video. In general, this is the information in the src element of an embed tag and should not be the same as the content of the loc tag.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### LinkField

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the text of the link

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the url of the link

</td>
</tr>
</tbody>
</table>

### ListPart

Represents a collection of content items.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItems</strong></td>
<td valign="top">[<a href="#contentitem">ContentItem</a>]</td>
<td>

the content items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n elements (10 by default)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of elements to skip

</td>
</tr>
</tbody>
</table>

### MarkdownBodyPart

Content stored as Markdown. You can also query the HTML interpreted version of Markdown.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>html</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the HTML representation of the markdown content

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>markdown</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the markdown value

</td>
</tr>
</tbody>
</table>

### MarkdownField

Content stored as Markdown. You can also query the HTML interpreted version of Markdown.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>html</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the HTML representation of the markdown content

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>markdown</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the markdown value

</td>
</tr>
</tbody>
</table>

### Markup

The markup of the Creative Work and its flavour

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>html</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The markup converted to HTML.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>markdown</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The markup converted to markdown.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>raw</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The markup unconverted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rawFlavor</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The flavour of the markup e.g. HTML, markdown etc.

</td>
</tr>
</tbody>
</table>

### Mass

Properties that take Mass as values are of the form '<Number> <Mass unit of measure>'. E.g., '7 kg'.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>measurment</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The measurment, such as Kg or mm.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>number</strong></td>
<td valign="top"><a href="#decimal">Decimal</a>!</td>
<td>

The value.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MaximumDose

The maximum dosing schedule considered safe for a drug or supplement as recommended by an authority or by the drug/supplement's manufacturer. Capture the recommending authority in the recognizingAuthority property of MedicalEntity.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MediaField

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>paths</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the media paths

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n elements

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the last n elements

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of elements to skip

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>urls</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the absolute urls of the media items

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">first</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the first n elements

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">last</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the last n elements

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">skip</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

the number of elements to skip

</td>
</tr>
</tbody>
</table>

### MedicalArticle

Represents a Medical Article.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>article</strong></td>
<td valign="top"><a href="#articlequery">ArticleQuery</a></td>
<td>

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalCondition</strong></td>
<td valign="top"><a href="#medicalcondition">MedicalCondition</a></td>
<td>

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### MedicalCode

A code for a medical entity.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A short textual code that uniquely identifies the value.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The coding system, e.g. 'ICD-10'.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalCondition

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>associatedAnatomy</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The anatomy of the underlying organ system or structures associated with this entity.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cause</strong></td>
<td valign="top">[<a href="#medicalsignorsymptom">MedicalSignOrSymptom</a>]</td>
<td>

Specifying a cause of something in general. e.g in medicine , one of the causative agent(s) that are most directly responsible for the pathophysiologic process that eventually results in the occurrence.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>epidemiology</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The characteristics of associated patients, such as age, gender, race etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>possibleTreatment</strong></td>
<td valign="top">[<a href="#medicaltherapy">MedicalTherapy</a>]</td>
<td>

A possible treatment to address this condition, sign or symptom.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryPrevention</strong></td>
<td valign="top"><a href="#medicaltherapy">MedicalTherapy</a></td>
<td>

A preventative therapy used to prevent an initial occurrence of the medical condition, such as vaccination.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>signOrSymptom</strong></td>
<td valign="top"><a href="#medicalsignorsymptom">MedicalSignOrSymptom</a></td>
<td>

A sign or symptom of this condition. Signs are objective or physically observable manifestations of the medical condition while symptoms are the subjective experience of the medical condition.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalDrugArticle

Represents a Medical Drug Article.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>article</strong></td>
<td valign="top"><a href="#articlequery">ArticleQuery</a></td>
<td>

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug</strong></td>
<td valign="top"><a href="#drug">Drug</a></td>
<td>

A chemical or biologic substance, used as a medical therapy, that has a physiological effect on an organism. Here the term drug is used interchangeably with the term medicine although clinical knowledge make a clear difference between them.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalCondition</strong></td>
<td valign="top"><a href="#medicalcondition">MedicalCondition</a></td>
<td>

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### MedicalEntity

The most generic type of entity related to health and the practice of medicine.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalIndication

A condition or factor that indicates use of a medical therapy, including signs, symptoms, risk factors, anatomical states, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalProcedure

A process of care used in either a diagnostic, therapeutic, preventive or palliative capacity that relies on invasive (surgical), non-invasive, or other techniques.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalSignOrSymptom

Any feature associated or not with a medical condition. In medicine a symptom is generally subjective while a sign is objective.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>associatedAnatomy</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The anatomy of the underlying organ system or structures associated with this entity.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cause</strong></td>
<td valign="top">[<a href="#medicalsignorsymptom">MedicalSignOrSymptom</a>]</td>
<td>

Specifying a cause of something in general. e.g in medicine , one of the causative agent(s) that are most directly responsible for the pathophysiologic process that eventually results in the occurrence.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>epidemiology</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The characteristics of associated patients, such as age, gender, race etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>possibleTreatment</strong></td>
<td valign="top">[<a href="#medicaltherapy">MedicalTherapy</a>]</td>
<td>

A possible treatment to address this condition, sign or symptom.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryPrevention</strong></td>
<td valign="top"><a href="#medicaltherapy">MedicalTherapy</a></td>
<td>

A preventative therapy used to prevent an initial occurrence of the medical condition, such as vaccination.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>signOrSymptom</strong></td>
<td valign="top"><a href="#medicalsignorsymptom">MedicalSignOrSymptom</a></td>
<td>

A sign or symptom of this condition. Signs are objective or physically observable manifestations of the medical condition while symptoms are the subjective experience of the medical condition.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalSpeciality

Any specific branch of medical science or practice. Medical specialities include clinical specialties that pertain to particular organ systems and their respective disease states, as well as allied health specialties. Enumerated type.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalTherapy

Any medical intervention designed to prevent, treat, and cure human diseases and medical conditions, including both curative and palliative therapies. Medical therapies are typically processes of care relying upon pharmacotherapy, behavioral therapy, supportive therapy (with fluid or nutrition for example), or detoxification (e.g. hemodialysis) aimed at improving or preventing a health condition.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indication</strong></td>
<td valign="top">[<a href="#medicalindication">MedicalIndication</a>]</td>
<td>

A factor that indicates use of this therapy for treatment and/or prevention of a condition, symptom, etc. For therapies such as drugs, indications can include both officially-approved indications as well as off-label uses. These can be distinguished by using the ApprovedIndication subtype of MedicalIndication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### MedicalWebpage

A web page that provides medical information.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### NutritionalInformation

Nutritional information about the recipe.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>calories</strong></td>
<td valign="top">[<a href="#energy">Energy</a>]</td>
<td>

The number of calories.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>carbohydrateContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

	The number of grams of carbohydrates.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cholesterolContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of milligrams of cholesterol.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fatContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of fat.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>fiberContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of fiber.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>proteinContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of protein.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>saturatedFatContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of saturated fat.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>servingSize</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The serving size, in terms of the number of volume or mass.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sodiumContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of milligrams of sodium.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sugarContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of sugar.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transFatContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of trans fat.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>unsaturatedContent</strong></td>
<td valign="top"><a href="#mass">Mass</a></td>
<td>

The number of grams of unsaturated fat.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Offer

An offer to transfer some rights to an item or to provide a service — for example, an offer to sell tickets to an event, to rent the DVD of a movie, to stream a TV show over the internet, to repair a motorcycle, or to loan a book.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>areaServed</strong></td>
<td valign="top"><a href="#geocoordinatesquery">GeoCoordinatesQuery</a></td>
<td>

The geographic area where a service or offered item is provided.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>itemOffered</strong></td>
<td valign="top"><a href="#servicequery">ServiceQuery</a></td>
<td>

The item being offered.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>offeredBy</strong></td>
<td valign="top"><a href="#organizationquery">OrganizationQuery</a></td>
<td>

A pointer to the organization or person making the offer.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>priceCurrency</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>priceSpecification</strong></td>
<td valign="top"><a href="#pricespecificationquery">PriceSpecificationQuery</a></td>
<td>

Detailed price specification, indicating the unit price and delivery or payment charges.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>seller</strong></td>
<td valign="top"><a href="#organizationquery">OrganizationQuery</a></td>
<td>

An entity which offers (sells / leases / lends / loans) the services / goods. A seller may also be a provider.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sku</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The Stock Keeping Unit (SKU), i.e. a merchant-specific identifier for a product or service, or the product to which the offer refers.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Organization

Represents a Organization.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#postaladdress">PostalAddress</a></td>
<td>

Physical address of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>areaServed</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The geographic area where a service or offered item is provided. 

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brand</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clinicalCommissioningGroup</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The ccg served by the organization or person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clinicalCommissioningGroupCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The code of the ccg served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dissolutionDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

The date that this organization was dissolved.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Email address.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ethicsPolicy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Statement about ethics policy.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>founder</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

A person who founded this organization.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundingDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

The date that this organization was founded.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>legalName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The official name of the organization, e.g. the registered company name.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="#place">Place</a></td>
<td>

The location of for example where the event is happening, an organization is located, or where an action takes place.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logo</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

An associated logo.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>makesOffer</strong></td>
<td valign="top">[<a href="#offer">Offer</a>]</td>
<td>

A pointer to products or services offered by the organization or person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>parentOrganization</strong></td>
<td valign="top"><a href="#organizationquery">OrganizationQuery</a></td>
<td>

The larger organization that this organization is a subOrganization of, if any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryCareTrust</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The primary care trust served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The publishingPrinciples property indicates (typically via URL) a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>strategicHealthAuthority</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The strategic health authority served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>taxID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>telephone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The telephone number.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vatID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Value-added Tax ID of the organization or person.

</td>
</tr>
</tbody>
</table>

### OrganizationQuery

An organization such as a school, NGO, corporation, club, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#postaladdress">PostalAddress</a></td>
<td>

Physical address of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>areaServed</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The geographic area where a service or offered item is provided. 

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>brand</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clinicalCommissioningGroup</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The ccg served by the organization or person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>clinicalCommissioningGroupCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The code of the ccg served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dissolutionDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

The date that this organization was dissolved.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Email address.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ethicsPolicy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Statement about ethics policy.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>founder</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

A person who founded this organization.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>foundingDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

The date that this organization was founded.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>legalName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The official name of the organization, e.g. the registered company name.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>location</strong></td>
<td valign="top"><a href="#place">Place</a></td>
<td>

The location of for example where the event is happening, an organization is located, or where an action takes place.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logo</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

An associated logo.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>makesOffer</strong></td>
<td valign="top">[<a href="#offer">Offer</a>]</td>
<td>

A pointer to products or services offered by the organization or person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>parentOrganization</strong></td>
<td valign="top"><a href="#organizationquery">OrganizationQuery</a></td>
<td>

The larger organization that this organization is a subOrganization of, if any.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>primaryCareTrust</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The primary care trust served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The publishingPrinciples property indicates (typically via URL) a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>strategicHealthAuthority</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The strategic health authority served by the organization or person

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>taxID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>telephone</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The telephone number.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vatID</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Value-added Tax ID of the organization or person.

</td>
</tr>
</tbody>
</table>

### PeopleAudience

A set of characteristics belonging to people, e.g. who compose an item's target audience.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audienceType</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The target group associated with a given audience (e.g. patients, medical professionals, etc.).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>geographicArea</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The geographic area associated with the audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalCondition</strong></td>
<td valign="top">[<a href="#medicalcondition">MedicalCondition</a>]</td>
<td>

Specifying the health condition(s) of a patient, medical study, or other target audience.

</td>
</tr>
</tbody>
</table>

### PersonQuery

A person (alive, dead, undead, or fictional).

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>accrediation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>additionalName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An additional name for a Person, can be used for a middle name.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Physical address of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>affiliation</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An organization that this person is affiliated with. For example, a school/university, a club, or a team.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alumniOf</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An organization that the person is an alumni of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>biography</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>birthDate</strong></td>
<td valign="top"><a href="#datetimeoffset">DateTimeOffset</a></td>
<td>

Date of birth.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>currentVersionAuthor</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Email address.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>familyName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Family name. In the U.S., the last name of an Person. This can be used along with givenName instead of the name property.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Gender of the person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>givenName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Given name. In the U.S., the first name of a Person. This can be used along with familyName instead of the name property.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>honorificPrefix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An honorific prefix preceding a Person's name such as Dr/Mrs/Mr.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>honorificSuffix</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

An honorific suffix preceding a Person's name such as M.D. /PhD/MSCSW.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

An image of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>jobTitle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The job title of the person (for example, Financial Manager).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>memberOf</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

An Organization to which this Person or Organization belongs.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nationality</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Nationality of the person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>peerReviewer</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shortBiography</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>telephoneNumber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The telephone number.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>worksFor</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td>

Organizations that the person works for.

</td>
</tr>
</tbody>
</table>

### Place

Entities that have a somewhat fixed, physical extension.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address</strong></td>
<td valign="top"><a href="#postaladdress">PostalAddress</a></td>
<td>

The mailing address.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>branchCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code (also called 'store code') that uniquely identifies a place of business. The code is typically assigned by the parentOrganization and used in structured URLs., For example, in the URL http://www.starbucks.co.uk/store-locator/etc/detail/3047 the code '3047' is a branchCode for a particular branch.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>geo</strong></td>
<td valign="top"><a href="#geocoordinatesquery">GeoCoordinatesQuery</a></td>
<td>

The Value-added Tax ID of the organization or person.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>logo</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

An associated logo.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publicAccess</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A flag to signal that the Place is open to public visitors. If this property is omitted there is no assumed default boolean value

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>smokingAllowed</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Indicates whether it is allowed to smoke in the place, e.g. in the restaurant, hotel or hotel room.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### PostalAddress

The mailing address.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>addressCountry</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The country. For example, USA. You can also provide the two-letter ISO 3166-1 alpha-2 country code.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>addressRegion</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The region. For example, CA.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postalCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The postal code. For example, 94043.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>streetAddress</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The street address. For example, 1600 Amphitheatre Pkwy.

</td>
</tr>
</tbody>
</table>

### PriceSpecificationQuery

A structured value representing a price or price range. Typically, only the subclasses of this type are used for markup. It is recommended to use MonetaryAmount to describe independent amounts of money such as a salary, credit card limits, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>commission</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deposit</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxPrice</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>minPrice</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>paymentDueType</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>price</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>priceCurrency</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>valueAddedTaxIncluded</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### PropertyValue

A property-value pair, e.g. representing a feature of a product or place.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The value of the quantitative value or property value node.

</td>
</tr>
</tbody>
</table>

### Quantity

Quantities such as distance, time, mass, weight, etc. Particular instances of say Mass are entities like '3 Kg' or '4 milligrams'.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>measurment</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The measurment, such as Kg or mm.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>number</strong></td>
<td valign="top"><a href="#decimal">Decimal</a>!</td>
<td>

The value.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Recipe

Represents a Recipe.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of creation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the latest version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of modification

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Is the published version

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

The date and time of publication

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recipe</strong></td>
<td valign="top"><a href="#recipequery">RecipeQuery</a></td>
<td>

A recipe. For dietary restrictions covered by the recipe, a few common restrictions are enumerated via suitableForDiet. The keywords property can also be used to add more detail.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### RecipeIngredient

A single ingredient used in the recipe, e.g. sugar, flour or garlic.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>allergies</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

List of allergies associated with this ingredient.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantities</strong></td>
<td valign="top">[<a href="#quantity">Quantity</a>]</td>
<td>

A single step item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sectionName</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### RecipeQuery

A recipe. For dietary restrictions covered by the recipe, a few common restrictions are enumerated via suitableForDiet. The keywords property can also be used to add more detail.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>allergies</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookingMethod</strong></td>
<td valign="top"><a href="#cookingmethod">CookingMethod</a></td>
<td>

A single step item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookTime</strong></td>
<td valign="top"><a href="#seconds">Seconds</a>!</td>
<td>

The time it takes to actually cook the dish, in ISO 8601 duration format.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dietTypeTagUrls</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>difficulty</strong></td>
<td valign="top"><a href="#recipedifficulty">RecipeDifficulty</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>enableImperialValues</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ingredientsTitleOverride</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lifestyleTagUrls</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lifestyleTypes</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nutrition</strong></td>
<td valign="top">[<a href="#nutritionalinformation">NutritionalInformation</a>]</td>
<td>

A single step item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nutritionalInformationBody</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nutritionalInformationTitleOverride</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recipeIngredient</strong></td>
<td valign="top">[<a href="#recipeingredient">RecipeIngredient</a>]</td>
<td>

A single step item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>servingUnit</strong></td>
<td valign="top"><a href="#servingunit">ServingUnit</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>strapline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suitableForDiet</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Indicates a dietary restriction or guideline for which this recipe or menu item is suitable, e.g. diabetic, halal etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

### SearchPromotion

Promoted search result.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>title</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### SearchResult

The search result.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItems</strong></td>
<td valign="top">[<a href="#contentitem">ContentItem</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queryTime</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relatedQueries</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>spellingSuggestions</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsoredResults</strong></td>
<td valign="top">[<a href="#searchpromotion">SearchPromotion</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>startIndex</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suggestedResults</strong></td>
<td valign="top">[<a href="#searchpromotion">SearchPromotion</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>totalResultCount</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### ServiceQuery

A service provided by an organization, e.g. delivery service, print services, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top">[<a href="#peopleaudience">PeopleAudience</a>]</td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isAlwaysFree</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isHidden</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>offers</strong></td>
<td valign="top">[<a href="#offer">Offer</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>providers</strong></td>
<td valign="top">[<a href="#organizationquery">OrganizationQuery</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Substance

Any matter of defined composition that has discrete existence, whose origin may be biological, mineral or chemical.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>activeIngredient</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

An active ingredient, typically chemical compounds and/or biologic substances.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### TherapeuticProcedure

A medical procedure intended primarily for therapeutic purposes, aimed at improving a health condition.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>code</strong></td>
<td valign="top">[<a href="#medicalcode">MedicalCode</a>]</td>
<td>

A medical code for the entity, taken from a controlled vocabulary or ontology such as ICD-9, DiseasesDB, MeSH, SNOMED-CT, RxNorm, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>indication</strong></td>
<td valign="top">[<a href="#medicalindication">MedicalIndication</a>]</td>
<td>

A factor that indicates use of this therapy for treatment and/or prevention of a condition, symptom, etc. For therapies such as drugs, indications can include both officially-approved indications as well as off-label uses. These can be distinguished by using the ApprovedIndication subtype of MedicalIndication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>releventSpeciality</strong></td>
<td valign="top">[<a href="#medicalspeciality">MedicalSpeciality</a>]</td>
<td>

If applicable, a medical specialty in which this entity is relevant.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Thing

The most generic type of item.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
</tbody>
</table>

### Webpage

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as breadcrumb may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternativeHeadline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

A secondary title of the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audience</strong></td>
<td valign="top"><a href="#audience">Audience</a></td>
<td>

An intended audience, i.e. a group for whom something was created.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

The author of this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contributor</strong></td>
<td valign="top">[<a href="#personororganization">PersonOrOrganization</a>]</td>
<td>

A secondary contributor to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightHolder</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The party holding the legal copyright to the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>copyrightYear</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The year during which the claimed copyright for the CreativeWork was first asserted.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>creator</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateCreated</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was created or the item was added to a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dateModified</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>datePublished</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date of first broadcast/publication.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>description</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A description of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>editor</strong></td>
<td valign="top"><a href="#personquery">PersonQuery</a></td>
<td>

Specifies the Person who edited the CreativeWork.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasPart</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>headline</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Headline of the article.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifier</strong></td>
<td valign="top">[<a href="#propertyvalue">PropertyValue</a>]</td>
<td>

The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inLanguage</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The language of the content or performance or used in an action..

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isFamilyFriendly</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates whether this content is family friendly.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>isPartOf</strong></td>
<td valign="top">[<a href="#creativework">CreativeWork</a>]</td>
<td>

Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>keywords</strong></td>
<td valign="top">[<a href="#string">String</a>!]!</td>
<td>

Keywords or tags used to describe this content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nextReviewed</strong></td>
<td valign="top"><a href="#date">Date</a></td>
<td>

The date on which the CreativeWork will next be reviewed.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>position</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The position of an item in a series or sequence of items.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>printableCopy</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

Document pdf path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishingPrinciples</strong></td>
<td valign="top"><a href="#uri">Uri</a>!</td>
<td>

The publishingPrinciples property indicates a document describing the editorial principles of an Organization (or individual e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reviewedBy</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

People or organizations that have reviewed the content on this web page for accuracy and/or completeness.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sameAs</strong></td>
<td valign="top">[<a href="#uri">Uri</a>!]!</td>
<td>

URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sponsor</strong></td>
<td valign="top"><a href="#personororganization">PersonOrOrganization</a></td>
<td>

An organization that supports a thing through a pledge, promise, or financial contribution. e.g. a sponsor of a Medical Study or a corporate sponsor of an event.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#markup">Markup</a></td>
<td>

The markup of the Creative Work and its flavour.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>thumbnailUrl</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

A thumbnail image relevant to the Thing.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timeRequired</strong></td>
<td valign="top"><a href="#seconds">Seconds</a></td>
<td>

Approximate or typical time it takes to work with or through this learning resource for the typical intended target audience.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>url</strong></td>
<td valign="top"><a href="#uri">Uri</a></td>
<td>

URL of the item.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlBase</td>
<td valign="top"><a href="#string">String</a></td>
<td>

the base url to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">urlKind</td>
<td valign="top"><a href="#urlkind">UrlKind</a></td>
<td>

the url kind to use when resolving urls

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>version</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

The version of the CreativeWork embodied by a specified resource.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>video</strong></td>
<td valign="top"><a href="#hubvideo">HubVideo</a></td>
<td>

A Video describe the recording, reproducing, or broadcasting of moving visual images.

</td>
</tr>
</tbody>
</table>

## Inputs

### ArticleInput

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
</tbody>
</table>

### ArticleOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### ArticleWhereInput

the Article content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#articlewhereinput">ArticleWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#articlewhereinput">ArticleWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#articlewhereinput">ArticleWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>webpage</strong></td>
<td valign="top"><a href="#webpagepartinput">WebpagePartInput</a></td>
<td>

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as breadcrumb may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

</td>
</tr>
</tbody>
</table>

### AuthorOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### AuthorWhereInput

the Author content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#authorwhereinput">AuthorWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#authorwhereinput">AuthorWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#authorwhereinput">AuthorWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
</tbody>
</table>

### ContainedPartInput

the list part of the content item

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>listContentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item id of the parent list of the content item to filter is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>listContentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item id of the parent list of the content item to filter is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>listContentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item id of the parent list of the content item to filter is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>listContentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item id of the parent list of the content item to filter is not in collection

</td>
</tr>
</tbody>
</table>

### DirectoryServiceOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### DirectoryServiceWhereInput

the DirectoryService content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#directoryservicewhereinput">DirectoryServiceWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#directoryservicewhereinput">DirectoryServiceWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#directoryservicewhereinput">DirectoryServiceWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
</tbody>
</table>

### HubOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### HubWhereInput

the Hub content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#hubwhereinput">HubWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#hubwhereinput">HubWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#hubwhereinput">HubWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>webpage</strong></td>
<td valign="top"><a href="#webpagepartinput">WebpagePartInput</a></td>
<td>

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as breadcrumb may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

</td>
</tr>
</tbody>
</table>

### MedicalArticleOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### MedicalArticleWhereInput

the MedicalArticle content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#medicalarticlewhereinput">MedicalArticleWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#medicalarticlewhereinput">MedicalArticleWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#medicalarticlewhereinput">MedicalArticleWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>article</strong></td>
<td valign="top"><a href="#articleinput">ArticleInput</a></td>
<td>

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalCondition</strong></td>
<td valign="top"><a href="#medicalconditionpartinput">MedicalConditionPartInput</a></td>
<td>

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalWebpage</strong></td>
<td valign="top"><a href="#medicalwebpagepartinput">MedicalWebpagePartInput</a></td>
<td>

A web page that provides medical information.

</td>
</tr>
</tbody>
</table>

### MedicalConditionPartInput

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A short textual code that uniquely identifies the value. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A short textual code that uniquely identifies the value. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The coding system, e.g. 'ICD-10'. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The coding system, e.g. 'ICD-10'. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not end with the string

</td>
</tr>
</tbody>
</table>

### MedicalDrugArticleOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### MedicalDrugArticleWhereInput

the MedicalDrugArticle content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#medicaldrugarticlewhereinput">MedicalDrugArticleWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#medicaldrugarticlewhereinput">MedicalDrugArticleWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#medicaldrugarticlewhereinput">MedicalDrugArticleWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>article</strong></td>
<td valign="top"><a href="#articleinput">ArticleInput</a></td>
<td>

An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types and this is intended to cover them all.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalCondition</strong></td>
<td valign="top"><a href="#medicalconditionpartinput">MedicalConditionPartInput</a></td>
<td>

Any condition of the human body that affects the normal functioning of a person, whether physically or mentally. Includes diseases, injuries, disabilities, disorders, syndromes, etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>medicalWebpage</strong></td>
<td valign="top"><a href="#medicalwebpagepartinput">MedicalWebpagePartInput</a></td>
<td>

A web page that provides medical information.

</td>
</tr>
</tbody>
</table>

### MedicalEntityPartInput

The most generic type of entity related to health and the practice of medicine.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A short textual code that uniquely identifies the value. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A short textual code that uniquely identifies the value. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codeValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A short textual code that uniquely identifies the value. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The coding system, e.g. 'ICD-10'. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The coding system, e.g. 'ICD-10'. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>codingSystem_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The coding system, e.g. 'ICD-10'. does not end with the string

</td>
</tr>
</tbody>
</table>

### MedicalWebpagePartInput

A web page that provides medical information.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Audience for which this web page is intended. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Audience for which this web page is intended. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not end with the string

</td>
</tr>
</tbody>
</table>

### OrganizationOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### OrganizationWhereInput

the Organization content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#organizationwhereinput">OrganizationWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#organizationwhereinput">OrganizationWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#organizationwhereinput">OrganizationWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
</tbody>
</table>

### RecipeOrderByInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentType</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>published</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>latest</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#orderbydirection">OrderByDirection</a></td>
<td></td>
</tr>
</tbody>
</table>

### RecipePartInput

A recipe. For dietary restrictions covered by the recipe, a few common restrictions are enumerated via suitableForDiet. The keywords property can also be used to add more detail.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookTime</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The time it takes to actually cook the dish, in ISO 8601 duration format. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookTime_not</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The time it takes to actually cook the dish, in ISO 8601 duration format. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookTime_in</strong></td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td>

The time it takes to actually cook the dish, in ISO 8601 duration format. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cookTime_not_in</strong></td>
<td valign="top">[<a href="#int">Int</a>]</td>
<td>

The time it takes to actually cook the dish, in ISO 8601 duration format. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>difficulty</strong></td>
<td valign="top"><a href="#recipedifficulty">RecipeDifficulty</a></td>
<td>

Difficulty of the recipe is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>difficulty_not</strong></td>
<td valign="top"><a href="#recipedifficulty">RecipeDifficulty</a></td>
<td>

Difficulty of the recipe is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>difficulty_in</strong></td>
<td valign="top">[<a href="#recipedifficulty">RecipeDifficulty</a>]</td>
<td>

Difficulty of the recipe is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>difficulty_not_in</strong></td>
<td valign="top">[<a href="#recipedifficulty">RecipeDifficulty</a>]</td>
<td>

Difficulty of the recipe is not in collection

</td>
</tr>
</tbody>
</table>

### RecipeWhereInput

the Recipe content item filters

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>contentItemId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

content item id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

content item id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not</strong></td>
<td valign="top"><a href="#id">ID</a></td>
<td>

the content item version id is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>contentItemVersionId_not_in</strong></td>
<td valign="top">[<a href="#id">ID</a>]</td>
<td>

the content item version id is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the display text of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>displayText_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the display text of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of creation is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>createdUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of creation is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of modification is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>modifiedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of modification is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

the date and time of publication is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>publishedUtc_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

the date and time of publication is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the owner of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>owner_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the owner of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

the author of the content item is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>author_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

the author of the content item does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>OR</strong></td>
<td valign="top">[<a href="#recipewhereinput">RecipeWhereInput</a>]</td>
<td>

OR logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>AND</strong></td>
<td valign="top">[<a href="#recipewhereinput">RecipeWhereInput</a>]</td>
<td>

AND logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>NOT</strong></td>
<td valign="top">[<a href="#recipewhereinput">RecipeWhereInput</a>]</td>
<td>

NOT logical operation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>webpage</strong></td>
<td valign="top"><a href="#webpagepartinput">WebpagePartInput</a></td>
<td>

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as breadcrumb may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>recipe</strong></td>
<td valign="top"><a href="#recipepartinput">RecipePartInput</a></td>
<td>

A recipe. For dietary restrictions covered by the recipe, a few common restrictions are enumerated via suitableForDiet. The keywords property can also be used to add more detail.

</td>
</tr>
</tbody>
</table>

### WebpagePartInput

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as breadcrumb may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>identifierName</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Name is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierName_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Name does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The Description is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>identifierValue_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The Description does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

The name of the item. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The name of the item. does not end with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_not</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_not_in</strong></td>
<td valign="top">[<a href="#datetime">DateTime</a>]</td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_gt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is greater than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_gte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is greater than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_lt</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is less than

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lastReviewed_lte</strong></td>
<td valign="top"><a href="#datetime">DateTime</a></td>
<td>

Date on which the content on this web page was last reviewed for accuracy and/or completeness. is less than or equal

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. is equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. is not equal to

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Audience for which this web page is intended. is in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_in</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Audience for which this web page is intended. is not in collection

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. contains the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_contains</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not contain the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. starts with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_starts_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not start with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. ends with the string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audienceType_not_ends_with</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Audience for which this web page is intended. does not end with the string

</td>
</tr>
</tbody>
</table>

## Enums

### DosageForm

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>TABLET</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SUSPENSION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>INJECTION</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SUPPOSITORY</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>TOPICAL</strong></td>
<td></td>
</tr>
</tbody>
</table>

### OrderByDirection

the order by direction

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ASC</strong></td>
<td>

orders content items in ascending order

</td>
</tr>
<tr>
<td valign="top"><strong>DESC</strong></td>
<td>

orders content items in descending order

</td>
</tr>
</tbody>
</table>

### PrescriptionStatus

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>PERSCRIPTION_ONLY</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OVER_THE_COUNTER</strong></td>
<td></td>
</tr>
</tbody>
</table>

### RecipeDifficulty

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>EASY</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>INTERMEDIATE</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DIFFICULT</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ServingUnit

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>G</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ML</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Status

publication status

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>PUBLISHED</strong></td>
<td>

published content item version

</td>
</tr>
<tr>
<td valign="top"><strong>DRAFT</strong></td>
<td>

draft content item version

</td>
</tr>
<tr>
<td valign="top"><strong>LATEST</strong></td>
<td>

the latest version, either published or draft

</td>
</tr>
<tr>
<td valign="top"><strong>ALL</strong></td>
<td>

all historical versions

</td>
</tr>
</tbody>
</table>

### UrlKind

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>identifier</strong></td>
<td>

Return urls as a contentitem identifier

</td>
</tr>
<tr>
<td valign="top"><strong>absolute</strong></td>
<td>

Returns urls as an absolute uri, requires baseUrl argument

</td>
</tr>
<tr>
<td valign="top"><strong>relative</strong></td>
<td>

Returns urls as a relative uri

</td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

### Date

The `Date` scalar type represents a year, month and day in accordance with the [ISO-8601](https://en.wikipedia.org/wiki/ISO_8601) standard.

### DateTime

The `DateTime` scalar type represents a date and time. `DateTime` expects timestamps to be formatted in accordance with the [ISO-8601](https://en.wikipedia.org/wiki/ISO_8601) standard.

### DateTimeOffset

The `DateTimeOffset` scalar type represents a date, time and offset from UTC. `DateTimeOffset` expects timestamps to be formatted in accordance with the [ISO-8601](https://en.wikipedia.org/wiki/ISO_8601) standard.

### Decimal

### Float

### ID

### Int

### Milliseconds

The `Milliseconds` scalar type represents a period of time represented as the total number of milliseconds.

### Seconds

The `Seconds` scalar type represents a period of time represented as the total number of seconds.

### String

### Uri
