<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guide Complet - Bloquer les Publicités sur Mobile</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        * {
            font-family: 'Inter', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .card-hover {
            transition: all 0.3s ease;
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .progress-bar {
            width: 0%;
            transition: width 0.5s ease;
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
            animation: fadeIn 0.3s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .comparison-before {
            background: linear-gradient(45deg, #ff6b6b, #ffa500);
        }
        
        .comparison-after {
            background: linear-gradient(45deg, #4ecdc4, #44a08d);
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header -->
    <header class="gradient-bg text-white py-16">
        <div class="container mx-auto px-6 text-center">
            <div class="mb-6">
                <span class="text-6xl">🛡️</span>
                <div class="mt-3">
                    <p class="text-lg font-medium text-white/90">par Anaja Meta</p>
                </div>
            </div>
            <h1 class="text-4xl md:text-6xl font-bold mb-4">Bloquez les Publicités</h1>
            <p class="text-xl md:text-2xl mb-8 opacity-90">Guide complet pour une navigation mobile sans interruption</p>
            <div class="bg-white/20 backdrop-blur-sm rounded-lg p-4 inline-block">
                <p class="text-lg">✅ Gratuit • ✅ Efficace • ✅ Facile à configurer</p>
            </div>
        </div>
    </header>

    <!-- Navigation rapide -->
    <nav class="bg-white shadow-lg sticky top-0 z-50">
        <div class="container mx-auto px-6">
            <div class="flex flex-wrap justify-center space-x-2 md:space-x-8 py-4">
                <button onclick="scrollToSection('solutions')" class="px-4 py-2 text-blue-600 hover:bg-blue-50 rounded-lg transition">Solutions</button>
                <button onclick="scrollToSection('guides')" class="px-4 py-2 text-blue-600 hover:bg-blue-50 rounded-lg transition">Guides</button>
                <button onclick="scrollToSection('comparison')" class="px-4 py-2 text-blue-600 hover:bg-blue-50 rounded-lg transition">Avant/Après</button>
                <button onclick="scrollToSection('advanced')" class="px-4 py-2 text-blue-600 hover:bg-blue-50 rounded-lg transition">Avancé</button>
            </div>
        </div>
    </nav>

    <!-- Statistiques importantes -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-4 gap-8 text-center">
                <div class="fade-in">
                    <div class="text-4xl font-bold text-red-500 mb-2">73%</div>
                    <p class="text-gray-600">de données économisées</p>
                </div>
                <div class="fade-in">
                    <div class="text-4xl font-bold text-green-500 mb-2">5x</div>
                    <p class="text-gray-600">plus rapide</p>
                </div>
                <div class="fade-in">
                    <div class="text-4xl font-bold text-blue-500 mb-2">90%</div>
                    <p class="text-gray-600">moins de distractions</p>
                </div>
                <div class="fade-in">
                    <div class="text-4xl font-bold text-purple-500 mb-2">2h</div>
                    <p class="text-gray-600">de batterie en plus</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Solutions principales -->
    <section id="solutions" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Solutions Recommandées</h2>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- AdGuard -->
                <div class="bg-white rounded-xl p-8 card-hover fade-in">
                    <div class="text-center mb-6">
                        <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="text-2xl">🛡️</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">AdGuard</h3>
                        <div class="flex justify-center mb-2">
                            <span class="text-yellow-400">★★★★★</span>
                        </div>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Bloque 99% des pubs</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Protection vie privée</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Fonctionne partout</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Interface simple</li>
                    </ul>
                    <button onclick="showGuide('adguard')" class="w-full bg-green-500 text-white py-3 rounded-lg hover:bg-green-600 transition font-medium">
                        Guide d'installation
                    </button>
                </div>

                <!-- Navigateurs avec bloqueur -->
                <div class="bg-white rounded-xl p-8 card-hover fade-in">
                    <div class="text-center mb-6">
                        <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="text-2xl">🌐</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">Brave Browser</h3>
                        <div class="flex justify-center mb-2">
                            <span class="text-yellow-400">★★★★☆</span>
                        </div>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Bloqueur intégré</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Gratuit à 100%</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Très rapide</li>
                        <li class="flex items-center"><span class="text-orange-500 mr-2">⚠</span> Seulement dans le navigateur</li>
                    </ul>
                    <button onclick="showGuide('brave')" class="w-full bg-blue-500 text-white py-3 rounded-lg hover:bg-blue-600 transition font-medium">
                        Guide d'installation
                    </button>
                </div>

                <!-- DNS -->
                <div class="bg-white rounded-xl p-8 card-hover fade-in">
                    <div class="text-center mb-6">
                        <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <span class="text-2xl">⚙️</span>
                        </div>
                        <h3 class="text-xl font-bold mb-2">DNS Filtrant</h3>
                        <div class="flex justify-center mb-2">
                            <span class="text-yellow-400">★★★☆☆</span>
                        </div>
                    </div>
                    <ul class="space-y-3 mb-6">
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Gratuit</li>
                        <li class="flex items-center"><span class="text-green-500 mr-2">✓</span> Fonctionne partout</li>
                        <li class="flex items-center"><span class="text-orange-500 mr-2">⚠</span> Configuration technique</li>
                        <li class="flex items-center"><span class="text-orange-500 mr-2">⚠</span> Moins efficace</li>
                    </ul>
                    <button onclick="showGuide('dns')" class="w-full bg-purple-500 text-white py-3 rounded-lg hover:bg-purple-600 transition font-medium">
                        Guide d'installation
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Guides détaillés -->
    <section id="guides" class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Guides d'Installation</h2>
            
            <!-- Onglets -->
            <div class="flex flex-wrap justify-center mb-8 bg-gray-100 rounded-lg p-2">
                <button onclick="showTab('adguard')" id="tab-adguard" class="tab-btn px-6 py-3 rounded-lg font-medium transition bg-white text-blue-600 shadow">AdGuard</button>
                <button onclick="showTab('brave')" id="tab-brave" class="tab-btn px-6 py-3 rounded-lg font-medium transition text-gray-600 hover:text-blue-600">Brave</button>
                <button onclick="showTab('dns')" id="tab-dns" class="tab-btn px-6 py-3 rounded-lg font-medium transition text-gray-600 hover:text-blue-600">DNS</button>
            </div>

            <!-- Contenu AdGuard -->
            <div id="content-adguard" class="tab-content active">
                <div class="max-w-4xl mx-auto">
                    <div class="bg-green-50 border border-green-200 rounded-lg p-6 mb-8">
                        <h3 class="text-xl font-bold text-green-800 mb-2">🏆 Solution Recommandée</h3>
                        <p class="text-green-700">AdGuard est la solution la plus complète et efficace pour bloquer les publicités sur mobile.</p>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">1</div>
                            <div>
                                <h4 class="font-bold mb-2">Télécharger AdGuard</h4>
                                <p class="text-gray-600 mb-3">Rendez-vous sur le site officiel adguard.com depuis votre téléphone</p>
                                <div class="bg-blue-100 p-3 rounded border-l-4 border-blue-500">
                                    <p class="text-sm"><strong>Important :</strong> Ne téléchargez jamais depuis le Play Store, utilisez uniquement le site officiel</p>
                                </div>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">2</div>
                            <div>
                                <h4 class="font-bold mb-2">Autoriser l'installation</h4>
                                <p class="text-gray-600 mb-3">Android vous demandera d'autoriser l'installation d'applications inconnues</p>
                                <ul class="text-sm text-gray-600 space-y-1">
                                    <li>• Allez dans Paramètres > Sécurité</li>
                                    <li>• Activez "Sources inconnues" temporairement</li>
                                    <li>• Ou autorisez juste pour votre navigateur</li>
                                </ul>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">3</div>
                            <div>
                                <h4 class="font-bold mb-2">Configuration initiale</h4>
                                <p class="text-gray-600 mb-3">Suivez l'assistant de configuration :</p>
                                <ul class="text-sm text-gray-600 space-y-1">
                                    <li>• Activez le filtrage HTTPS</li>
                                    <li>• Autorisez le VPN local</li>
                                    <li>• Choisissez vos filtres (recommandé : tous)</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Contenu Brave -->
            <div id="content-brave" class="tab-content">
                <div class="max-w-4xl mx-auto">
                    <div class="bg-blue-50 border border-blue-200 rounded-lg p-6 mb-8">
                        <h3 class="text-xl font-bold text-blue-800 mb-2">🌐 Solution Simple</h3>
                        <p class="text-blue-700">Brave est un navigateur avec bloqueur de publicités intégré, parfait pour débuter.</p>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">1</div>
                            <div>
                                <h4 class="font-bold mb-2">Télécharger Brave</h4>
                                <p class="text-gray-600 mb-3">Disponible gratuitement sur Google Play Store et App Store</p>
                                <div class="flex space-x-4">
                                    <div class="bg-green-100 px-3 py-1 rounded text-sm">✓ Play Store</div>
                                    <div class="bg-green-100 px-3 py-1 rounded text-sm">✓ App Store</div>
                                </div>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">2</div>
                            <div>
                                <h4 class="font-bold mb-2">Configuration</h4>
                                <p class="text-gray-600 mb-3">Le bloqueur est activé par défaut, mais vous pouvez l'optimiser :</p>
                                <ul class="text-sm text-gray-600 space-y-1">
                                    <li>• Menu ⋮ > Paramètres > Brave Shields</li>
                                    <li>• Activez "Blocage agressif"</li>
                                    <li>• Bloquez les scripts et cookies</li>
                                </ul>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center font-bold">3</div>
                            <div>
                                <h4 class="font-bold mb-2">Définir par défaut</h4>
                                <p class="text-gray-600 mb-3">Pour une protection complète :</p>
                                <ul class="text-sm text-gray-600 space-y-1">
                                    <li>• Paramètres Android > Applications par défaut</li>
                                    <li>• Choisir Brave comme navigateur par défaut</li>
                                    <li>• Tous les liens s'ouvriront dans Brave</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Contenu DNS -->
            <div id="content-dns" class="tab-content">
                <div class="max-w-4xl mx-auto">
                    <div class="bg-purple-50 border border-purple-200 rounded-lg p-6 mb-8">
                        <h3 class="text-xl font-bold text-purple-800 mb-2">⚙️ Solution Technique</h3>
                        <p class="text-purple-700">Configuration DNS pour bloquer les publicités au niveau réseau.</p>
                    </div>
                    
                    <div class="space-y-6">
                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-purple-500 text-white rounded-full flex items-center justify-center font-bold">1</div>
                            <div>
                                <h4 class="font-bold mb-2">Accéder aux paramètres WiFi</h4>
                                <p class="text-gray-600 mb-3">Sur votre réseau WiFi actuel :</p>
                                <ul class="text-sm text-gray-600 space-y-1">
                                    <li>• Paramètres > WiFi</li>
                                    <li>• Appuyez longuement sur votre réseau</li>
                                    <li>• Sélectionnez "Modifier le réseau"</li>
                                </ul>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-purple-500 text-white rounded-full flex items-center justify-center font-bold">2</div>
                            <div>
                                <h4 class="font-bold mb-2">Configurer DNS</h4>
                                <p class="text-gray-600 mb-3">Remplacez les DNS par :</p>
                                <div class="bg-gray-800 text-green-400 p-3 rounded font-mono text-sm">
                                    DNS 1: 176.103.130.130<br>
                                    DNS 2: 176.103.130.131
                                </div>
                                <p class="text-xs text-gray-500 mt-2">DNS AdGuard avec filtrage publicitaire</p>
                            </div>
                        </div>

                        <div class="flex items-start space-x-4 p-4 bg-gray-50 rounded-lg">
                            <div class="w-8 h-8 bg-purple-500 text-white rounded-full flex items-center justify-center font-bold">3</div>
                            <div>
                                <h4 class="font-bold mb-2">Alternatives DNS</h4>
                                <p class="text-gray-600 mb-3">Autres serveurs DNS filtrants :</p>
                                <div class="space-y-2 text-sm">
                                    <div class="bg-white p-2 rounded border">
                                        <strong>CleanBrowsing:</strong> 185.228.168.9 / 185.228.169.9
                                    </div>
                                    <div class="bg-white p-2 rounded border">
                                        <strong>Quad9:</strong> 9.9.9.9 / 149.112.112.112
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Comparaison avant/après -->
    <section id="comparison" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Avant / Après</h2>
            
            <div class="grid md:grid-cols-2 gap-8 max-w-6xl mx-auto">
                <!-- Avant -->
                <div class="comparison-before rounded-xl p-8 text-white">
                    <h3 class="text-2xl font-bold mb-6 text-center">😤 AVANT</h3>
                    <div class="space-y-4">
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-red-300 mr-2">⏱️</span>
                                <span class="font-medium">Temps de chargement</span>
                            </div>
                            <div class="text-2xl font-bold">8-15 secondes</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-red-300 mr-2">📱</span>
                                <span class="font-medium">Consommation data</span>
                            </div>
                            <div class="text-2xl font-bold">100% normale</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-red-300 mr-2">🔋</span>
                                <span class="font-medium">Batterie</span>
                            </div>
                            <div class="text-2xl font-bold">Drain rapide</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-red-300 mr-2">😵</span>
                                <span class="font-medium">Expérience</span>
                            </div>
                            <div class="text-2xl font-bold">Frustrante</div>
                        </div>
                    </div>
                </div>

                <!-- Après -->
                <div class="comparison-after rounded-xl p-8 text-white">
                    <h3 class="text-2xl font-bold mb-6 text-center">😍 APRÈS</h3>
                    <div class="space-y-4">
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-green-300 mr-2">⚡</span>
                                <span class="font-medium">Temps de chargement</span>
                            </div>
                            <div class="text-2xl font-bold">2-3 secondes</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-green-300 mr-2">📊</span>
                                <span class="font-medium">Consommation data</span>
                            </div>
                            <div class="text-2xl font-bold">-73% économie</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-green-300 mr-2">🔋</span>
                                <span class="font-medium">Batterie</span>
                            </div>
                            <div class="text-2xl font-bold">+2h autonomie</div>
                        </div>
                        
                        <div class="bg-white/20 p-4 rounded-lg">
                            <div class="flex items-center mb-2">
                                <span class="text-green-300 mr-2">😊</span>
                                <span class="font-medium">Expérience</span>
                            </div>
                            <div class="text-2xl font-bold">Fluide & rapide</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Conseils avancés -->
    <section id="advanced" class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Conseils Avancés</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gradient-to-br from-blue-50 to-blue-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">🔒</div>
                    <h3 class="text-xl font-bold mb-3">Protection Vie Privée</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• Bloquez les trackers</li>
                        <li>• Désactivez la géolocalisation</li>
                        <li>• Utilisez un VPN si nécessaire</li>
                        <li>• Videz régulièrement le cache</li>
                    </ul>
                </div>

                <div class="bg-gradient-to-br from-green-50 to-green-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">⚡</div>
                    <h3 class="text-xl font-bold mb-3">Optimisation Performance</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• Activez la compression</li>
                        <li>• Bloquez les images lourdes</li>
                        <li>• Désactivez JavaScript si possible</li>
                        <li>• Utilisez le mode sombre</li>
                    </ul>
                </div>

                <div class="bg-gradient-to-br from-purple-50 to-purple-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">🛠️</div>
                    <h3 class="text-xl font-bold mb-3">Configuration Réseau</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• Configurez votre routeur</li>
                        <li>• Utilisez Pi-hole à la maison</li>
                        <li>• Bloquez au niveau FAI</li>
                        <li>• Filtres personnalisés</li>
                    </ul>
                </div>

                <div class="bg-gradient-to-br from-orange-50 to-orange-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">📱</div>
                    <h3 class="text-xl font-bold mb-3">Applications Spécifiques</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• YouTube Vanced (Android)</li>
                        <li>• uBlock Origin (Firefox)</li>
                        <li>• Blokada (open source)</li>
                        <li>• NextDNS (cloud)</li>
                    </ul>
                </div>

                <div class="bg-gradient-to-br from-red-50 to-red-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">⚠️</div>
                    <h3 class="text-xl font-bold mb-3">Précautions</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• Évitez les apps douteuses</li>
                        <li>• Ne payez pas pour du gratuit</li>
                        <li>• Vérifiez les permissions</li>
                        <li>• Sauvegardez vos paramètres</li>
                    </ul>
                </div>

                <div class="bg-gradient-to-br from-teal-50 to-teal-100 p-6 rounded-xl card-hover">
                    <div class="text-3xl mb-4">🎯</div>
                    <h3 class="text-xl font-bold mb-3">Listes de Filtres</h3>
                    <ul class="text-sm space-y-2 text-gray-700">
                        <li>• EasyList (international)</li>
                        <li>• Liste FR (français)</li>
                        <li>• Anti-malware</li>
                        <li>• Réseaux sociaux</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ -->
    <section class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Questions Fréquentes</h2>
            
            <div class="max-w-4xl mx-auto space-y-4">
                <div class="bg-white rounded-lg shadow-sm">
                    <button onclick="toggleFaq(1)" class="w-full p-6 text-left flex justify-between items-center hover:bg-gray-50">
                        <span class="font-medium">Est-ce légal de bloquer les publicités ?</span>
                        <span class="faq-icon">+</span>
                    </button>
                    <div id="faq-1" class="faq-content hidden px-6 pb-6">
                        <p class="text-gray-600">Oui, c'est parfaitement légal. Vous avez le droit de contrôler ce qui s'affiche sur votre appareil. C'est comme changer de chaîne TV pendant les pubs.</p>
                    </div>
                </div>

                <div class="bg-white rounded-lg shadow-sm">
                    <button onclick="toggleFaq(2)" class="w-full p-6 text-left flex justify-between items-center hover:bg-gray-50">
                        <span class="font-medium">Cela va-t-il casser certains sites web ?</span>
                        <span class="faq-icon">+</span>
                    </button>
                    <div id="faq-2" class="faq-content hidden px-6 pb-6">
                        <p class="text-gray-600">Très rarement. Les bloqueurs modernes sont intelligents. Si un site ne fonctionne pas, vous pouvez facilement le débloquer temporairement.</p>
                    </div>
                </div>

                <div class="bg-white rounded-lg shadow-sm">
                    <button onclick="toggleFaq(3)" class="w-full p-6 text-left flex justify-between items-center hover:bg-gray-50">
                        <span class="font-medium">Quelle est la différence entre les solutions ?</span>
                        <span class="faq-icon">+</span>
                    </button>
                    <div id="faq-3" class="faq-content hidden px-6 pb-6">
                        <p class="text-gray-600">AdGuard bloque partout (apps + navigateur), Brave seulement dans le navigateur, DNS au niveau réseau mais moins précis.</p>
                    </div>
                </div>

                <div class="bg-white rounded-lg shadow-sm">
                    <button onclick="toggleFaq(4)" class="w-full p-6 text-left flex justify-between items-center hover:bg-gray-50">
                        <span class="font-medium">Cela consomme-t-il plus de batterie ?</span>
                        <span class="faq-icon">+</span>
                    </button>
                    <div id="faq-4" class="faq-content hidden px-6 pb-6">
                        <p class="text-gray-600">Au contraire ! En bloquant les publicités gourmandes, vous économisez de la batterie. Gain moyen de 2h d'autonomie.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6 text-center">
            <div class="mb-8">
                <span class="text-4xl">🛡️</span>
                <div class="mt-2 mb-3">
                    <p class="text-sm text-gray-400">par Anaja Meta</p>
                </div>
                <h3 class="text-2xl font-bold mb-2">Navigation Sans Limites</h3>
                <p class="text-gray-400">Profitez d'internet comme il devrait être : rapide, propre et respectueux.</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8 mb-8">
                <div>
                    <h4 class="font-bold mb-3">Avantages</h4>
                    <ul class="text-sm text-gray-400 space-y-1">
                        <li>Navigation 5x plus rapide</li>
                        <li>73% de données économisées</li>
                        <li>Protection vie privée</li>
                        <li>Batterie préservée</li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-3">Solutions</h4>
                    <ul class="text-sm text-gray-400 space-y-1">
                        <li>AdGuard (recommandé)</li>
                        <li>Brave Browser</li>
                        <li>DNS filtrant</li>
                        <li>Extensions navigateur</li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold mb-3">Support</h4>
                    <ul class="text-sm text-gray-400 space-y-1">
                        <li>Guides détaillés</li>
                        <li>Configuration pas à pas</li>
                        <li>Conseils avancés</li>
                        <li>FAQ complète</li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 pt-8">
                <p class="text-gray-400 text-sm">
                    Guide éducatif sur le blocage de publicités • Toutes les solutions présentées sont gratuites et légales
                </p>
                <p class="text-gray-500 text-xs mt-2">© 2025 Anaja Meta - Développé avec passion</p>
            </div>
        </div>
    </footer>

    <script>
        // Animation au scroll
        function animateOnScroll() {
            const elements = document.querySelectorAll('.fade-in');
            elements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('visible');
                }
            });
        }

        // Scroll fluide vers section
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({
                behavior: 'smooth'
            });
        }

        // Gestion des onglets
        function showTab(tabName) {
            // Cacher tous les contenus
            document.querySelectorAll('.tab-content').forEach(content => {
                content.classList.remove('active');
            });
            
            // Désactiver tous les boutons
            document.querySelectorAll('.tab-btn').forEach(btn => {
                btn.classList.remove('bg-white', 'text-blue-600', 'shadow');
                btn.classList.add('text-gray-600');
            });
            
            // Activer le contenu sélectionné
            document.getElementById('content-' + tabName).classList.add('active');
            
            // Activer le bouton sélectionné
            const activeBtn = document.getElementById('tab-' + tabName);
            activeBtn.classList.add('bg-white', 'text-blue-600', 'shadow');
            activeBtn.classList.remove('text-gray-600');
        }

        // Guide rapide
        function showGuide(type) {
            showTab(type);
            scrollToSection('guides');
        }

        // FAQ
        function toggleFaq(num) {
            const content = document.getElementById('faq-' + num);
            const icon = content.previousElementSibling.querySelector('.faq-icon');
            
            if (content.classList.contains('hidden')) {
                content.classList.remove('hidden');
                icon.textContent = '−';
            } else {
                content.classList.add('hidden');
                icon.textContent = '+';
            }
        }

        // Barre de progression de lecture
        function updateProgressBar() {
            const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            const scrolled = (winScroll / height) * 100;
            
            if (document.querySelector('.progress-bar')) {
                document.querySelector('.progress-bar').style.width = scrolled + '%';
            }
        }

        // Event listeners
        window.addEventListener('scroll', () => {
            animateOnScroll();
            updateProgressBar();
        });

        window.addEventListener('load', () => {
            animateOnScroll();
        });

        // Animation des statistiques au chargement
        function animateStats() {
            const stats = [
                { element: document.querySelectorAll('.fade-in')[0].querySelector('.text-4xl'), target: 73 },
                { element: document.querySelectorAll('.fade-in')[1].querySelector('.text-4xl'), target: 5 },
                { element: document.querySelectorAll('.fade-in')[2].querySelector('.text-4xl'), target: 90 },
                { element: document.querySelectorAll('.fade-in')[3].querySelector('.text-4xl'), target: 2 }
            ];

            stats.forEach((stat, index) => {
                setTimeout(() => {
                    let current = 0;
                    const increment = stat.target / 50;
                    const timer = setInterval(() => {
                        current += increment;
                        if (current >= stat.target) {
                            current = stat.target;
                            clearInterval(timer);
                        }
                        
                        if (index === 0 || index === 2) {
                            stat.element.textContent = Math.floor(current) + '%';
                        } else if (index === 1) {
                            stat.element.textContent = Math.floor(current) + 'x';
                        } else {
                            stat.element.textContent = Math.floor(current) + 'h';
                        }
                    }, 50);
                }, index * 200);
            });
        }

        // Démarrer l'animation des stats après un délai
        setTimeout(animateStats, 1000);
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9792429477b0c765',t:'MTc1Njg3MTE4Ni4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
