<?xml version="1.0" encoding="UTF-8"?>
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
	<xsl:output method="xml" indent="yes"/>

	<xsl:template match="/">
		<xsl:apply-templates select="payoff_quote_inquiry"/>
	</xsl:template>

	<xsl:template match="payoff_quote_inquiry">
		<payoff_quote_inquiry>
			<Product>
				<xsl:value-of select="@Product"/>
			</Product>
			<idtype>
				<xsl:value-of select="@idtype"/>
			</idtype>
			<idvalue>
				<xsl:value-of select="@idvalue"/>
			</idvalue>
			<tempqname>
				<xsl:value-of select="@tempqname"/>
			</tempqname>
			<requested_good_until_date>
				<xsl:value-of select="@requested_good_until_date"/>
			</requested_good_until_date>
			<Current_or_next_month>
				<xsl:value-of select="@Current_or_next_month"/>
			</Current_or_next_month>
			<dealertrack_dealerid>
				<xsl:value-of select="@dealertrack_dealerid"/>
			</dealertrack_dealerid>
			<lender_dealerid>
				<xsl:value-of select="@lender_dealerid"/>
			</lender_dealerid>
			<verified>
				<xsl:value-of select="@verified"/>
			</verified>
		</payoff_quote_inquiry>
	</xsl:template>

</xsl:stylesheet>
