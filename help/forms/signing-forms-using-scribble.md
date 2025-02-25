---
title: Apply electronic signatures to a form using scribble signatures
seo-title: Apply electronic signatures to a form using scribble signatures
description: Signing forms using scribble
seo-description: Signing forms using scribble
uuid: ffeba886-9b24-4ed1-95c0-e19356ff2f23
products: SG_EXPERIENCEMANAGER/6.5/FORMS
topic-tags: author
discoiquuid: 76d178d1-8e40-41b3-80d4-66b2f8d04211
docset: aem65
google-site-verification: A1dSvxshSAiaZvk0yHu7-S3hJBb1THj0CZ2Uh8N_ck4
exl-id: dc89ecb1-2d9e-4d1d-b85b-af90c550e7d8
---
# Apply electronic signatures to a form using scribble signatures{#apply-electronic-signatures-to-a-form-using-deprecated-scribble-signatures}

You can use the **Scribble Signature** component and **Signature Step** component to draw (Scribble) signature on an Adaptive Form. The Signature step component displays a PDF version of the Adaptive Form. You require a Document of Record option enabled or form template based Adaptive Forms to use the Signature step component.

Both the components provide a window, as displayed below, to sign a form. You can also click the geolocation icon ![aem_6_3_geolocation](assets/aem_6_3_geolocation.png) to add geolocation to the signature.

![Scribble sign dialog](assets/scribble-signature.png)

## Configure an Adaptive Form to use Scribble Signature {#configure-an-adaptive-form-to-use-scribble-signature}

1. Create a Document of Record option enabled or form template based Adaptive Form. For step-by-step information, see [Creating an Adaptive Form](creating-adaptive-form.md).
1. Drag-and-drop the **Scribble Signature** component from component browser to the Adaptive Form.
1. Tap the **Configure** ![configure](assets/configure.png) icon. It opens properties browser and displays properties of the Scribble Signature component. Configure properties of the Scribble Signature component.
1. Drag-and-drop the Signature Step component from component browser to the Adaptive Form.

   >[!NOTE]
   >
   >The Signature Step component takes up full width available for the form. It is recommended to not have any other component on the section containing the Signature Step component.

1. In the Content browser, tap **Form Container**, and tap the **Configure** ![](assets/configure.png) icon. It opens properties browser and displays Adaptive Form container properties. Navigate to **Adaptive Form Container** &gt; **Electronic Signature** and deselect the **Enable Adobe Sign** option. Tap the Done ![aem_6_3_forms_save](assets/aem_6_3_forms_save.png) icon to save the changes.

   >[!NOTE]
   >
   >When you add a Signature Step component to an Adaptive Form, the Enable Adobe Sign option is selected automatically.

1. Tap the **Configure** ![configure](assets/configure.png) icon. It opens properties browser and displays Signature step properties. Configure the following properties:

    * **Element Name**: Specify name of the component.

    * **Title:** Specify unique title of the component.
    * **Template message:** Specify the message to be displayed while the signature PDF is being loaded. Adobe Sign services take some time to prepare and load signature PDF.
    * **Signing Service:** Select the **Scribble Signature** option.

    * **CSS Class**: Specify CSS class of the client library, if any. It is recommended to use [themes](themes.md) and [in-line styles](inline-style-adaptive-forms.md) instead of CSS Class.

   Tap the Done ![aem_6_3_forms_save](assets/aem_6_3_forms_save.png) icon to save the changes. The Signature is configured sucessfully.

   Now, when you fill a form, a PDF version of Adaptive Form is displayed and options to sign the PDF document are provided. For detailed information, see [Sign an Adaptive Form using Scribble Signature](signing-forms-using-scribble.md#sign-an-adaptive-form-using-scribble-signature).

## Sign an Adaptive Form using Scribble Signature {#sign-an-adaptive-form-using-scribble-signature}

1. After you fill an Adaptive Form and reach the Signature Step page, the signature screen is displayed.

   ![Signature screen for EchoSign page](assets/esignscribblesign.jpg)

1. Click **[!UICONTROL Sign]**. The scribble sign dialog appears. Sign the form and click the Done ![aem_6_3_forms_save](assets/aem_6_3_forms_save.png) icon to save the signature.

   ![Scribble sign dialog](assets/scribblewidget.jpg)

1. Click complete to finish the signing process.

   ![Complete the signing process](assets/scribblecomplete.jpg)

The signatures are added to the form and the form control moves to the next panel.
