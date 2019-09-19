---
author: Mamaylya
description: Learn about the do's and don'ts for a successful mixed reality guide created in Dynamics 365 Guides
ms.author: mamaylya
ms.date: 10/01/2019
ms.service: crm-online
ms.topic: article
title: How to make a good mixed reality guide in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# How to make a great mixed reality guide

Other online documentation in Dynamics 365 Guides focuses on helping you learn how to use the Dyanmics 365 Guides applications and their various features. This document focuses on how to author great guide content to best communicate instructions to your operators. We suggest reading all other documentation first to get a good understanding of how to use the Dynamics 365 Guides applications, and then refer to this documentation to start authoring high-quality guides.

## Get started

### Gather content

Gather as much content as you can before you begin creating your guide. This includes images, videos, and 3D content (if you have any), 
and the physical objects themselves (if feasible). Don’t worry if you don’t have any 3D content. Guides includes a 3D Toolkit 
(including simple models such as arrows, hands, zones, etc.) that you can use to get started.

### Understand the space

Make sure you understand the space, the procedure, and the workflow you’re authoring for. Arrange for access to the space so you 
understand the real-world environment. You’ll also need access to the space to align the guide and place holograms later.

### Build references

A great way to start is to create a video of the procedure you want to show, or have someone (an expert in that process, for 
example) create one for you. You can refer to the video as you create your guide. If you’re using a video as a starting point, 
make sure it’s representative of the guide you want to create. For example, are you creating a guide for an expert or a novice?

### Understand your lesson objectives and target audience

It is critical to understand your lesson objectives and target audience before developing your guide. Lesson objectives include 
various sub-objectives that are needed to accomplish an overall Guides objective. Additionally, understanding your target 
population will help you tailor your guide to provide the right amount of complexity needed to communicate information to your 
operators. For example, will your audience understand how to use specific tools, or the names of specific machinery?

## What features can you use as an author to make a good guide?

Guide Structure

Tasks:
•	When first organizing a guide’s structure, break the assembly process into logical "Key Objectives, i.e. "Tasks."

  –	Think about tasks as key "check points" throughout the guide.
  
  –	At the end of each task, the operator should accomplish one significant goal.
  
•	Tasks should include only one main objective. If a task contains more than one main objective, break it into two or more tasks. 
This will help the operator retain the organization of the guide, leading to better retention.

•	Tasks should follow a logical sequence of actions.

•	When starting to write a guide, talk the assembly process "out loud"- i.e. how would you verbally communicate this process 
to someone in person?

•	To provide overall context, add an “Overview” and/or “Welcome” task at the start of the guide.

   –	This task can include the following steps:

      •	A step that describes what the guide is about.

      •	A step with a list of all the tasks that within the guide. This will help set a road map of the assembly process to the operator 
and lead to better retention.

      •	If safety is a critical concern, you can add an additional step focused on specific safety measures you would like the operators 
to take before beginning the guide.

***EXAMPLE IMAGE HERE***

•	Tasks shouldn't be more than 30 steps. If a task contains more than 30 steps break it into two or more tasks.

    –	Our research shows that having too many steps on a single task can start to overwhelm an operator, especially if this is their 
first time learning the procedure.

Steps:

•	Unlike traditional instructions, step text in Guides isn't meant to describe everything because you have additional visual aids 
such as images, videos, and 3D holograms.

   –	When writing a step consider all the different forms of communication you are using.
   
   –	Try to stick to one type of asset (image, video, or 3D hologram) per step. Too much media or 3D content can be overwhelming to 
   the operator and too time-consuming to absorb. Think about what type of content gets your point across best.
   
   –	In general, operators will read the text, look at images or videos, follow the dotted line, and observe 3D holograms. 
   Keep this order of operations in mind when writing a step.
   
•	It's critical to keep your audience in mind when writing a step.

   –	Will your audience know the names of specific tools are and what they can do?
   
      •	If yes, you can use less detail and don't need to explain what tools or parts are.
      
      •	If no, you should add extra descriptions and clarifying visuals to support operators.
      
      •	For a general audience, describe unique things (Custom parts or tools) and don't describe generic things (generic tools).
      
   –	Will your audience understand basic safety requirements?
   
   –	Will you audience understand different environmental cues and conditions?
   
•	Don’t be afraid to add lots of steps

   –	Remember to keep steps short for the best effect.
   
   –	If you have multiple sentences in a single step, our research shows that operators will often read the first sentence, 
   try to complete the action, and miss the rest of the content on the step.
   
   –	***EXAMPLE IMAGE HERE***
   
   –	In this example, many operators might miss the second sentence and continue onto the next step.

•	Keep text simple and colloquial

   –	Don’t be verbose
   
   –	Write your guide in colloquial human language for best results. Don’t use technical jargon that people don’t know or understand.

   –	Try to cut out unnecessary words.

   –	Make sure to use language the intended audience will understand.

   –	On PC, you will get a warning if your text is going to go over the 280-character limit. If you are approaching the 280-character 
limit, this is a good indication that you are trying to put too much information on a single step.

   –	We do not currently support any text formatting (Such as font size or styling) within Guides, but you can use capitalization to 
point out key words or phrases.

   –	Adding numbered or multiple small steps inside a single step can often lead an operator to miss specific actions. Don’t be afraid 
to create separate steps to make sure the operator completes the correct sequence of actions.

•	Use descriptive action words like “locate,” “find,” “get,” “go to”, “pick up,” “put down,” “insert,” “attach,” and “remove.”

•	Keep language consistent throughout the entire guide. Items that are especially important for language consistency include:

   –	Part names
   
   –	Action verbs
   
   –	Referring to Task names
   
•	Consider adding additional separate steps that show individual tips and tricks.

   –	Adding tips/tricks onto an action step can often lead the operator to miss them.
   
       •	It can be beneficial to add the tip/tricks as a separate step before the action step.
       
       •	Adding a NOTE step is useful for quality checks. This type of step can come before or after another step, depending on the 
       specific context.
       
       ***EXAMPLE IMAGE HERE***
       
       •	Add a WARNING step for things that could be dangerous or cause a quality issue. This type of step can come before or after 
       another step, depending on the specific context. On HoloLens, you can add a warning style on a 3D hologram to reinforce the 
       warning step text.
       
       ***EXAMPLE IMAGE HERE***
       
•	Add a step at the end of each task to let the operator know that they’re ending a task and introduce them to the following 
       task. This will help the operator form a mental model of the guide structure, leading to better retention.
       
•	If it isn't a generic tool/part (i.e. screwdriver, socket wrench, washer etc.), make sure to label and define the tool/part 
       the first time you introduce it to the operator
       
       –	After labeling and describing it the first time, you do not need to define it throughout the rest of the Guide.
       
•	Validation: If certain actions are critical to the success of subsequent actions, make sure to put a validation step in. Some 
validation examples include:

       –	Visual Validation
       
          •	"Make sure the green side is facing up"
          
          •	"Make sure the text is upside down when screwing it in"
          
          •	"Make sure the front of the machine is facing you and aligns to the top right corner of the table before continuing on to 
          the next step."
          
       –	Auditory Validation
       
          •	"Twist the knob to the right until you hear 2 loud clicks."
          
       –	Reference Validation
       
          •	" Reference image for correct orientation before continuing on to the next step. The following steps rely on correct 
          orientation of the circuit box."
          
•	Hands:

         Do not specify which hand to use (left/right) unless:
  
          •	Using a specific hand is important to the process (i.e. "Hold the left side down with your left hand, and use your right hand to 
turn the knob simultaneously")

          •	Strength is required

             –	If strength is required, make sure to specify dominant/non-dominant hand in the step instructions (i.e. "Turn the knob three times with your dominant hand. It will require force.")

## The Dotted Line

•	The main purpose of the dotted line is to spatially locate the operator where the work will be taking place.

•	You *should* use the dotted line when:

  –	Starting a guide. This well help orient the operator at the right general location where the work will take place.
  
  –	When moving to a different area on a new step.
  
  –	When locating a part.
  
  –	When moving to a different area of a large piece of machinery (i.e. grater than 2' away from the previous step).
  
•	You *should not* use the dotted line on every step.

  –	Using the dotted line to point to the same location over multiple steps can become visual clutter distracting the operator from focusing on 3D holograms or the physical piece of machinery.
  
•	Do not use the dotted line to point to a specific location (within 10mm). Instead use the dotted line to orient the operator to a general area, and then place a 3D hologram (an arrow, for example) at the end of the dotted line to point to a more specific location.

•	Use the tether for "Part Pickup" in the following ways:

–	For the first time picking up a part, use the tether to show the operator where it is.

–	For the second time, or to put a tool back, you don't need to use the tether again (Unless it's in a different location).

## 2D Images

We recommend using 2D images in the following scenarios:

•	"What to do & What not to do"

   –	When operators do something the wrong way consistently, it's useful to have an image in the "correct way" next to an image of the "incorrect way" highlighting the key difference.

   ***EXAMPLE IMAGE HERE***

•	Validation

  –	Orientation Validation

    •	Using an image is a clear way to make sure parts or machinery are in the correct orientation. This can be critically important if subsequent steps are based on correct orientation of a specific part or piece.
    
      –	Make sure to give enough environmental context to visually communicate to operators the correct orientation in the environment.
      
      ***EXAMPLE IMAGE HERE***


      –	Part Validation
      
      •	Use images for part identification in cases where a work-station has multiple parts that could be confused with one another visually---This is especially useful when two or more parts looks very similar with one minute differences.      

      •	Validating that an operator is picking up the correct part by comparing it to a picture or reference number

•	General notes for images:

     –	Make sure images:
     
        •	Clear
        
        •	High quality (1080p is recommended. 4K images are unnecessary)
        
        •	Capture enough context to orient the operator contextually in the environment.
        
        ***EXAMPLE IMAGE HERE***
        
        •	From the viewpoint of how the operator will see it.

        •	Don't contain extra visual noise that can confuse or distract the operator from what you are trying to communicate.

        •	Images should maintain 16:9 ratio to fill the entire media panel.

        •	Images should not be taken from too far away that the operator can't see enough detail of what you are trying to communicate.

        •	Make sure to preview all images in HoloLens before using a Guide (Image detail and color may appear different on HoloLens).

•	If an image is critical, say ***REFER TO IMAGE*** before any additional action text in the step instructions. If you put it after an action text operators can miss it- You can even put this as it's own step before the action to make sure the user pays attention to the image.

   ***EXAMPLE IMAGE HERE***

## Videos

We recommend using videos for:

   •	Unique interactions
   
     –	Detailed hand processes.
     
     –	Steps where millimeter accuracy is critical, and 3D holograms may not be accurate enough.
     
     –	Processes where standard holograms are too abstract, but custom holograms are too complex for your team to produce.
     
   •	Videos should be shot from a 3rd person or 1st person perspective.
   
      ***EXAMPLE IMAGE  OF 3RD-PERSON VS 1ST-PERSON HERE***

     –	3rd Person works best for:
     
        •	Show environmental context of where you are doing the work.

        •	Understand how to the operator and machine are interacting.

        •	When filming in 3rd person, it helps to start wide (to see full context) and then zoom in to understand detailed operations.

        •	3rd person videos can easily be taken with any hand-held camera.

     –	1st Person works best for:

        •	Small tight spaces

        •	Fine hand work

        •	When communicating the work from the perspective of the operator is critical to the success of the procedure.

        •	For 1st-person videos, we recommend mounting a camera to the authors head using a GoPro or similar device.

•	Only show how to do something one way (i.e. don't show alternative methods)

    –	Showing multiple ways to complete a step may be confusing to operators learning the task— pick the best method of completing the step and only communicate this method to operators
    
## 3D Toolkit

3D Toolkit Categories:

Arrows

•	Use arrows to communicate simple spatial information like position, direction, and translation.

•	Use arrows when you want the operator to insert a part into something.

   –	Arrows are great to pointing to a specific location (Within a +/- 2mm tolerance)

   –	Arrows can be used to show directionality (i.e. "Twist the lever until tight"--with corresponding half circle arrow showing movement direction)

   –	You can use a combination of different arrows to show a sequence of different actions (i.e. "Swing then pull")- This can also be paired with numbers (Expanded upon here)

   –	You can use arrows in combination with other 3D holograms (for example, checks and cross’) to show where to put something and where not to put something.

      ***EXAMPLE IMAGE HERE***

Hands

•	Hands are best to communicate specific hand orientations or movements.

•	Use hands when you want the operator to use their hands in a specific way to grab or manipulate something. There are various poses for specific interactions that are available in the 3D Toolkit such as Pull, Push, Pinch, Grab, etc.

     –	Combine these hands with arrows and/or additional 3D holograms to add additional meaning.

•	Generally, the "Pick Up" or “Place” shader works best with hands allowing operators to visually align their hands with the hologram.

Numbers

•	Numbers should be used for sequencing within a step

   –	Example: "First pull the lever (1) and then place it in the key hole (2)."

      ***EXAMPLE IMAGE HERE***

•	Numbers should not be used to identify parts in the world

    –	Example: "Pick up the screwdriver (1) and the socket wrench (2)."

•	Numbers should not be used to communicate how many of something to get

    –	Example: "Pick up 3 screws." --- Holographic Number 3 is next to screws

Zones

•	Zones are a good way to communicate areas to place items.

   ***EXAMPLE IMAGE HERE***

•	Zones can be used to show the orientation and location of objects.

•	Animated zones are effective in getting operators attention.

•	If you are using zones to communicate orientation, it is helpful to pair it with a reference image.

   ***EXAMPLE IMAGE HERE***

Generic Tools

•	Generic tools can be used in two ways:

   –	Symbols

     •	Use the scaled-down version of a generic tool (For example, screw driver) next to a real world part to indicate to the operator the type of tool to pick-up or use

   –	Models
   
     •	Use a scaled up version of a generic tool to indicate to the operator the actual scale of a specific tool to pick-up or use

Symbols

•	The "Check" and "Cross" symbols are best at communicating where to and where not where not to:

   •	Place things

   •	Run things through

   •	Clearance areas

   •	Which part of machinery or tool to select out of an array of options.

•	The "Exclamation Point" is best at communicating critical or alarming information

   •	We recommend using the "Exclamation Point" with the "Avoid" or “Warning “style.

   •	Do not overuse the "Exclamation Point," as it will lose its urgency after repeated use.

•	The "Lighting Bolt" is best at communication potential electrical hazards

•	We recommend using the "Lighting Bolt" with the “Avoid” or "Warning" style.

## Custom 3D Holograms

•	In general, try to accomplish a step by using 3D Toolkit. If you cannot achieve the desired result with 3D Toolkit assets, you can use a custom asset, image, or video instead.

•	Use custom high-fidelity assets where details matter and custom low-fidelity assets for high-level principles where details aren’t as important.

    •	Example- if detailed accuracy is important, like a referencing a specific port or lever, highly detailed custom assets may be necessary.

    •	If you are trying to show how to align the object, a general shape may achieve the desired effect.

•	Custom assets are best at communicating unique parts or unusual animation behaviors.

•	Animated custom holograms are a great way to show the flow or movement patters throughout a step.

•	You should use a custom hologram of the entire object for orientation and alignment steps.

•	You can always use a combination of custom assets with the 3D Toolkit on any step.

## Hologram Styles

•	Use styles to help create a visual hierarchy of 3D holograms

•	Use styles consistently to communicate specific actions. If you use styles consistently, as operators continue to use Guides, they will start to understand what styles are intended to mean, which will speed up their learning process.

Hologram Style Options:

Original

•	For 3D Toolkit assets, the "Original" shader is a white material

   –	The original white material is a good generic style because it doesn’t have any strong pre-existing connotations for operators.

   –	If your focus is more on alignment or positioning, the original shader is a good choice because it won’t have any strong action indications to the operator.

•	For custom assets, the "Original" shader is whatever is imported with the 3D model.

   –	Depending on the Authors needs or requirements, you can import a custom model with any style on it. Some good examples might include:

      •	Specific colors on sections of a model to identify parts or pieces.

         –	You can then add step instructions that refer to the colored sections.

         ***EXAMPLE IMAGE HERE***

      •	Realistic style to show what the actual object looks like

Pick Up

•	The pick-up style shows an outline around the hologram.

•	We recommend using the Pick-Up style for:

    –	Having the operator pick up a part/piece.

       •	This works especially well on:

          –	The hands holograms in the 3D Toolkit because operators can align their hand to the hologram, positioning their hand in the right orientation and position.

          –	Picking up parts because the outline around the real-world object visually distinguishes it from the rest of the environment.

Place

•	Place style is similar to the Pick-Up style but has a dashed outline instead of a solid outline.

•	We recommend using the place style for:

   –	Trying to align a real-world object to a hologram, because operators can place the real object in the hologram to validate that it visually matches.

See-Through (Two Options – 1 + 2)

•	"See-Through" is best at de-emphasizing holograms in the world because it makes the hologram semi-transparent and darker.

•	When creating a visual hierarchy of Holograms, "See-Through" can be used to soften less important holograms in the scene.

   ***EXAMPLE IMAGE HERE***

•	See-Through 1 is less opaque than See-Through 2.

Warning

•	Warning style is yellow and black stripes which is synonymous with warning.

•	 You should use a warning style when a hologram represents something that is potentially:

   –	Dangerous
   
   –	Electric
   
   –	Hazardous

Avoid

•	Avoid is a red pulsing style that should be used when:

   –	Trying to avoid touching or interacting with a specific zone or part.
   
   –	Something is dangerous or electrical (Can also use warning style based on specific context).

   –	Trying to avoid a clearance area.

X-Ray

•	X-ay resembles the effect of an x-ray scan.

•	X-Ray should be used when a hologram is placed within another object, helping the operator understand the depth order of parts.

Metal

•	The Metal style represents a highly glossy metal and can be used to give a hologram a realistic shinny material.

## Anchoring

•	Place the anchor on the base object (Rather than a static object such as a table or cart), so if orientation of the base object is incorrect, the operator can rescan and correct hologram positions.

   ***EXAMPLE IMAGE HERE***

•	Important orientation that could impact alignment of future steps be coupled with visual guides either via photo or custom hologram and text reminders to check their positioning.

   ***EXAMPLE IMAGE HERE***

•	Make sure to explain anchoring fundamentals to operators, otherwise they may be confused how to fix it if they incorrectly align a real object.

### See Also

[Author a guide](authoring-overview.md)<br>
[Operator's manual](operator-guide.md)<br>
[Analyze your guides](analytics-guide.md)<br>
[FAQ](faq.md)<br>
[Known issues]
