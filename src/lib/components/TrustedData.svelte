<script>
    const partners = [
        { name: "Fivetran", icon: "F", color: "bg-blue-600" },
        { name: "Snowflake", icon: "❄️" },
        { name: "Amazon Redshift", icon: "A", color: "bg-orange-600" },
        { name: "Google BigQuery", icon: "G", color: "bg-blue-500" },
        { name: "Microsoft Fabric", icon: "M", color: "bg-blue-700" },
        { name: "dbt", icon: "d", color: "bg-orange-500" },
        { name: "Power BI", icon: "P", color: "bg-yellow-600" },
        { name: "Tableau", icon: "T", color: "bg-blue-400" },
        { name: "Looker", icon: "L", color: "bg-purple-600" },
        { name: "Asana", icon: "A", color: "bg-pink-500" },
        { name: "Jira", icon: "J", color: "bg-blue-600" },
        { name: "Slack", icon: "S", color: "bg-purple-700" }
    ];
</script>

<section class="py-24 bg-white">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16 max-w-2xl">
            <h2 class="text-3xl md:text-4xl font-serif text-gray-900 mb-6">Modern Data Stack</h2>
            <p class="text-sm text-gray-500 leading-relaxed">
                We work with industry-leading tools and platforms to build robust, scalable data infrastructure. Our expertise spans the entire modern data stack, from integration to visualization.
            </p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            {#each partners as partner}
                <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                    <div class={`h-8 w-8 rounded flex items-center justify-center text-white text-xs font-bold ${partner.color ? partner.color : 'bg-gray-200 text-gray-600'}`}>
                        {partner.icon}
                    </div>
                    <span class="text-sm font-medium text-gray-900">{partner.name}</span>
                </div>
            {/each}
        </div>
    </div>
</section>
