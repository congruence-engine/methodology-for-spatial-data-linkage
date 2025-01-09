# Disambiguationg historic mill sites

## Short summary
Methodology developed in collaboration with Historic England (HE) for disambiguating mill sites across 3 (HE) datasets (Listed Buildings, Records and the Gazetteer).

## Research questions
1) What types of computational techniques are required to disambiguate sites? 
2) What sorts of software would be required to achieve the disambiguation?  
3) Is it possible to disambiguate sites using spatial methods only?
4) Can disambiguation be achieved solely through programmatic means or is a human reviewer necessary?
5) What are the key issues to be aware of in performing disambiguation?

## People 
**Nayomi Kasthuri Arachchi**: Methodology, Writing - original draft

**Daniel Belteki**: Methodology 

**Matthew Bristow (HE)**: Methodology, Resources

**Simon Crutchley (HE)**: Methodology, Resources

**Alex Butterworth**: Conceptualization, Supervision

## Data
The following datasets from HE:
- Listed buildings
- Records
- Gazetteer

## Method
We developed a two-stage method that consisted of spatial disambiguation followed by string matching. 

The spatial disambiguation phase involved creating carefully specified buffers around buildings appearing in HE datasets. These buffers could then be overlaid on grid references of sites. Any grid references falling within a buffer region could be considered potential duplicates of the point around which the buffer was originally drawn. 

Applying the spatial process sequentially to the listed buildings, Historic Environment Record and Gazetteer datasets would eventually leave a residual dataset containing grid references that didn't fall within the perimeters of any of the buffers drawn in the spatial disambiguation process. These residual points could then be disambiguated through a combination of text fuzzy matching and grid reference matching to a specified number of digits.

## Outputs
- a_method_for_geospatial_mapping.docx: document listing the steps in the methodology 

## Key initial findings

## Challenges

## Licence 
This work is licensed under a [Creative Commons Attribution 4.0 License - CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
