# PowerShell ISE Snippets

## Demo
![image](https://raw.github.com/dfinke/ISESnippets/master/images/demo.gif)

## I put my snippets here

	$snippetPath = Join-Path (Split-Path $profile.CurrentUserCurrentHost) "Snippets"
	$null = mkdir $snippetPath

Here is one that creates a PSCustomObject from a hash table. The snippet below inserts this, with the caret position set on the second line, indented and ready for typing. 

	[PSCustomObject] @{
	    
	}

## Snippet XML


	<?xml version='1.0' encoding='utf-8' ?>
	    <Snippets  xmlns='http://schemas.microsoft.com/PowerShell/Snippets'>
	        <Snippet Version='1.0.0'>
	            <Header>
	                <Title>PSCustomObject</Title>
	                <Description>Creates a new object</Description>
	                <Author>Doug Finke</Author>
	                <SnippetTypes>
	                    <SnippetType>Expansion</SnippetType>
	                </SnippetTypes>
	            </Header>
	
	            <Code>
	                <Script Language='PowerShell' CaretOffset='24'>
	                    <![CDATA[[PSCustomObject] @{
	
					}]]>
	                </Script>
	            </Code>
	
	    </Snippet>
	</Snippets>